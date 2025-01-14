---
layout: "lesson"
lang: "ml"
title: "പ്രമാണവർഗ്ഗങ്ങൾക്കു് രൂപകല്പനയിലെ സ്വാധീനം"
description: "ഈ പാഠം പ്രമാണവർഗ്ഗങ്ങൾ എന്താണെന്നും അവ എങ്ങനെ പ്രമാണത്തിന്റെ രൂപകല്പനയെ സ്വാധീനിക്കുന്നുവെന്നും വിശദമാക്കുന്നു. അതുകൂടാതെ, വിവിധതരം ടെൿ വിതരണങ്ങളിൽ ലഭ്യമായ പ്രധാന പ്രമാണവർഗ്ഗങ്ങളെപ്പറ്റിയുള്ള വിവരവും നൽകുന്നു."
toc-anchor-text: "പ്രമാണവർഗ്ഗങ്ങൾ"
toc-description: "പ്രമാണങ്ങളുടെ രൂപഘടന ക്രമീകരിക്കൽ."
---


# പ്രമാണവർഗ്ഗങ്ങൾ

<span class="summary"> പ്രമാണവർഗ്ഗങ്ങൾ എന്താണെന്നും അവ എങ്ങനെ പ്രമാണത്തിന്റെ രൂപകല്പനയെ സ്വാധീനിക്കുന്നുവെന്നും വിശദമാക്കുന്നതോടൊപ്പം വിവിധതരം ടെൿ വിതരണങ്ങളിൽ ലഭ്യമായ പ്രധാന പ്രമാണവർഗ്ഗങ്ങളെപ്പറ്റിയുള്ള വിവരവും ഈ പാഠം നമുക്കു് നൽകുന്നു.</span>


എല്ലാ ലാറ്റെൿ പ്രമാണങ്ങളും തുടങ്ങുന്നതു തന്നെ `\documentclass` എന്ന ആജ്ഞയോടുകൂടിയാണു് എന്ന കാര്യം നിങ്ങൾ ഇതിനിടെ ശ്രദ്ധിച്ചിരിക്കും. മിക്കവാറും അതു് `\documentclass{article}` എന്ന രീതിയിലുള്ളതായിരിക്കും. എങ്കിലും നമ്മൾ [കഴിഞ്ഞ പാഠത്തിൽ](lesson-04) അദ്ധ്യായത്തിന്റെ ശീർഷക നിർമ്മിതിക്കായി `\documentclass{report}` എന്നും ഒരിക്കൽ ഉപയോഗിക്കുകയുണ്ടായി. ഒരു ലാറ്റെൿ പ്രമാണത്തിന്റെ ആദ്യവരി മിക്കവാറും എല്ലായ്പോഴും ഈ ആജ്ഞകൊണ്ടു തന്നെയാവണം തുടങ്ങേണ്ടതു് എന്നും മനസ്സിലാക്കുക.


## എന്താണു് ഒരു പ്രമാണവർഗ്ഗം ചെയ്യുന്നതു്?

പ്രമാണവർഗ്ഗങ്ങൾ പേരു സൂചിപ്പിക്കുന്നപോലെ പ്രമാണങ്ങളുടെ സാമാന്യേനയുള്ള വിന്യാസക്രമത്തെ നിർവ്വചിക്കുന്നു. ഉദാഹരണമായി,

- രൂപകല്പന: മാർജിനുകൾ, ലിപിസഞ്ചയങ്ങൾ, ശൂന്യസ്ഥലവിനിയോഗം, മുതലായവ
- അദ്ധ്യായങ്ങൾ ഉണ്ടോ എന്ന കാര്യം 
- പ്രമാണത്തിന്റെ ശീർഷകം തനിയെ വേറൊരു താളിലാണോ എന്നതു്

പ്രമാണവർഗ്ഗങ്ങൾ അവയ്ക്കു് മാത്രമായുള്ള പ്രത്യേകതരം ആജ്ഞകളും അതിന്റെ പ്രയോഗക്രമങ്ങളും നിർവ്വചിക്കുകകൂടി ചെയ്യുന്നു. ഉദാഹരണമായി അവതരണങ്ങൾക്കു് (presentations) വേണ്ടി എഴുതപ്പെട്ട ഒരു വർഗ്ഗം അതിന്റെ വിന്യാസം സുഗമവും പ്രയത്നരഹിതവുമാക്കുന്ന തരത്തിലുള്ള ആജ്ഞകളാൽ സമ്പന്നമാണു്.

<!---കോഷ്‌ഠചിഹ്നം, ആവരണചിഹ്നം, വലയചിഹ്നം --->

പ്രമാണമാസകലം പ്രയോഗിക്കാവുന്ന തരത്തിലുള്ള _സാർവലൗകിക ഐച്ഛികങ്ങൾ_ (global options) നിർവ്വചിക്കുവാൻ ഈ വർഗ്ഗങ്ങൾക്കു് കഴിയും. അത്തരം ഐച്ഛികങ്ങളെ കോഷ്ഠചിഹ്നങ്ങൾക്കുള്ളിലാണു (square brackets) സാധാരണയായി നൽകുക: `\documentclass[<options>]{<class_name>}`. കോഷ്ഠചിഹ്നങ്ങളിൽ ഐച്ഛികങ്ങൾ ഉള്ളടക്കം ചെയ്തുകൊണ്ടുള്ള ഈ ആജ്ഞാഘടന പല ലാറ്റെൿ ആജ്ഞകളിലും സർവസാധാരണമായി ഉപയോഗിക്കുന്ന ഒരു രീതിയുമാണു്.

  
## അടിസ്ഥാനവർഗ്ഗങ്ങൾ 

ലാറ്റെക്കിൽ ഒരു നിര പ്രമാണവർഗ്ഗങ്ങൾ ലഭ്യമാണു്.  മിക്കവാറും അവയൊക്കെ ഒരേതരത്തിലുള്ള ആജ്ഞകളാൽ പൂരിതമാണു്, ചില്ലറ വ്യത്യാസങ്ങൾ അവതമ്മിൽ ഉണ്ടെങ്കിൽപ്പോലും.

- `article`  
  അദ്ധ്യായങ്ങളില്ലാത്ത ചെറിയ പ്രമാണങ്ങൾ 
- `report`  
  അദ്ധ്യായങ്ങൾ ഉള്ള നീണ്ട പ്രമാണങ്ങൾ, താളിന്റെ രണ്ടുപുറങ്ങളും ഒന്നുപോലെ വിന്യസിച്ചതു്
- `book`  
  നീണ്ട പ്രമാണങ്ങൾ, രണ്ടുവശങ്ങളും വ്യത്യസ്തമായ വിന്യാസം, മുൻ, മദ്ധ്യ, പിൻഭാഗങ്ങൾ (സൂചിക തുടങ്ങിയവ ഉള്ളടക്കം ചെയ്യുന്നതാണു പിൻഭാഗം) ഉള്ള പ്രമാണങ്ങൾ  
- `letter`  
  കത്തിടപാടിനു്, ഖണ്ഡങ്ങളില്ലാത്തതു്
- `slides`  
  അവതരണങ്ങൾക്കു് 


മുമ്പു് നമ്മൾ മനസ്സിലാക്കിയതുപോലെ, `article`, `report`, `book` എന്നീ വർഗ്ഗങ്ങൾ ഏതാണ്ടു് ഒരേ മാതിരിയുള്ള ആജ്ഞകൾ ഉള്ളടക്കം ചെയ്യുന്നു. പക്ഷെ, `letter` എന്ന വർഗ്ഗത്തിൽ വളരെ വ്യത്യസ്തമായ ആജ്ഞകളാണുള്ളതു്.

```latex
\documentclass{letter}
\usepackage[T1]{fontenc}
\begin{document}

\begin{letter}{Some Address\\Some Street\\Some City}

\opening{Dear Sir or Madam,}

The text goes Here

\closing{Yours,}

\end{letter}

\end{document}
```


മേൽവിലാസത്തിലെ വരികൾ മുറിക്കാൻ ``\\`` എന്ന ആജ്ഞ പ്രയോഗിച്ചിരിക്കുന്നതു് മുകളിൽ കൊടുത്ത ഉദാഹരണത്തിൽ കണ്ടുവല്ലോ. [അല്പം കഴിഞ്ഞിട്ടു്](lesson-11) വരികൾ മുറിക്കുന്ന വിദ്യ നമുക്കു് മനസ്സിലാക്കാം. കൂടാതെ, `letter` എന്ന വർഗ്ഗത്തിൽ പുതിയ പരിസരങ്ങളും (environments) സവിശേഷമായ ആജ്ഞകളും നിർവ്വചിക്കുകകൂടി ചെയ്തിരിക്കുന്ന കാര്യവും ശ്രദ്ധിക്കുക.


അടിസ്ഥാനവർഗ്ഗങ്ങളായ `article`, `report`, `book` എന്നീ മൂന്നു വർഗ്ഗങ്ങൾക്കൊപ്പം `10pt`,
`11pt`, `12pt` എന്ന ഐച്ഛികങ്ങൾ ലിപിയുടെ വലിപ്പം മാറ്റാനും, `twocolumn` എന്നതു് രണ്ടു കോളമായി പ്രമാണമാസകലം വിന്യസിക്കാനും ഉപയോഗിക്കാവുന്നതാണു്. 


## കർമ്മസമൃദ്ധമായ പ്രമാണവർഗ്ഗങ്ങൾ

ലാറ്റെക്കിലുള്ള അടിസ്ഥാനവർഗ്ഗങ്ങൾ ഒരിക്കലും പ്രശ്നങ്ങളൊന്നും സൃഷ്ടിക്കാത്ത, വളരെ സുസ്ഥിരമായവയാണു്. ആ കാരണം കൊണ്ടു് അവയിൽ ലഭ്യമായ വിന്യാസസൗകര്യങ്ങളുടെ കാര്യത്തിൽ ഒരുതരം യാഥാസ്ഥിതികത്വം പുലർത്തുന്നതായി തോന്നാം. അങ്ങനെ തന്നെയാണു് ആജ്ഞകളുടെ എണ്ണം, വ്യാപ്തി എന്നിവയുടെ കാര്യവും. ഈ ന്യൂനത പരിഹരിക്കാൻ, കാലാന്തരത്തിൽ ഒട്ടനവധി ശക്തമായ, കർമ്മസമൃദ്ധമായ ആജ്ഞകളും പരിസരങ്ങളും പ്രദാനം ചെയ്യുന്ന എണ്ണമറ്റ പ്രമാണവർഗ്ഗങ്ങൾ സൃഷ്ടിക്കപ്പെട്ടു. പ്രമാണത്തിന്റെ ആദ്യവരിയിൽ കൊടുത്തിരിക്കുന്ന വർഗത്തിന്റെ പേർ മാറ്റിയാൽ മാത്രം മതി, വിവിധതരത്തിൽ വിന്യസിക്കപ്പെട്ട പ്രമാണങ്ങൾ നമുക്കു് ഒറ്റ പാഠസ്രോതസ്സിൽ നിന്നു് അനായാസേന സൃഷ്ടിക്കാൻ കഴിയും. ഈ കാര്യത്തെക്കുറിച്ചു് വിശദമായി [പിന്നാലെ വേറൊരു പാഠത്തിൽ](lesson-11) നമ്മൾ പഠിക്കാനിരിക്കുകയാണു്.


അടിസ്ഥാനവർഗ്ഗങ്ങളായ `article`, `book` എന്നിവയ്ക്കു് പകരം ഇവയുടെ വകഭേദങ്ങൾ യഥാക്രമം `amsart`, `amsbook` എന്നീ പേരുകളുള്ള രണ്ടു പ്രമാണവർഗ്ഗങ്ങൾ അമേരിക്കൻ മാത്തമാറ്റിക്കൽ സൊസൈറ്റി പ്രസിദ്ധീകരിക്കുകയുണ്ടായി. ഇവ ഗണിതശാസ്ത്ര ഗവേഷണ ജേണലുകളിൽ പൊതുവെ പിന്തുടരുന്ന ശൈലിയോടു് വളരെ അടുത്തുനിൽക്കുന്ന രീതിയിൽ പാഠവിന്യാസം നടത്തുവാൻ സഹായിക്കുന്നവയാണു്. 

വളരെ ജനപ്രീതിയാർജ്ജിച്ച, വലിപ്പമേറിയ, വ്യാപകമായ വിന്യാസസൗകര്യങ്ങളുള്ള രണ്ടു് വർഗ്ഗങ്ങളാണു് കോമ-സ്ക്രിപ്റ്റ് (KOMA-Script), മെമ്വാര്‍ (memoir) എന്നിവ. കോമ-സ്ക്രിപ്റ്റ് ഒരു നിര പ്രമാണവർഗ്ഗങ്ങൾ ലാറ്റെക്കിന്റെ അടിസ്ഥാനവർഗ്ഗങ്ങൾക്കു് സമാനമായ രീതിയിൽ പ്രദാനം ചെയ്യുന്നു --- `scrartcl`, `scrreprt`, `scrbook`, `scrlttr2`. നേരെ മറിച്ചു് മെമ്വാറാകട്ടെ വിവിധാംശനിർമ്മിതമായ എന്തുതരം ഉള്ളടക്കത്തെയും, പുസ്തകങ്ങളെയും വിന്യസിക്കാൻ കെല്പുള്ള ഒറ്റ ബൃഹത്തായ പ്രമാണവർഗ്ഗമായി നിലകൊള്ളുന്നു.


ഈ കർമ്മവർദ്ധിത പ്രമാണവർഗ്ഗങ്ങൾ പാഠത്തെ നമ്മുടെ ഇച്ഛാനുസരണം വിന്യസിക്കുവാനുള്ള സൂത്രവിദ്യകളും ആജ്ഞാനിരകളും നൽകുന്നുണ്ടു്. ഇതിൽപ്പെട്ട ചില വസ്തുതകൾ നമ്മൾ അഭ്യാസത്തിൽ പരിശോധിക്കുയും ചെയ്യുന്നു. ഈ വർഗ്ഗങ്ങളുടെ വിശേഷാൽ കഴിവുകളെ നമുക്കെങ്ങനെ മനസ്സിലാക്കാം എന്നോർത്തു് വ്യാകുലപ്പെടേണ്ട, നമ്മൾ [പിന്നാലെ വരുന്ന ഒരു പാഠത്തിൽ](lesson-16) പഠിക്കാൻ പോകുകയാണു്, എന്നിരിക്കിലും അതിനു കാത്തുനിൽക്കാതെ നിങ്ങൾക്കു് വേണമെങ്കിൽ മുന്നോട്ടു് ചെല്ലാവുന്നതാണു്. 


## അവതരണങ്ങൾ 

`slides` എന്ന വർഗ്ഗം എഴുതപ്പെട്ടതു് 1980-കളിൽ അവതരണത്തിനു് വേണ്ട സ്ലൈഡുകൾ അച്ചടിക്കാനാണു്.  അതുകൊണ്ടു് ഇന്നത്തെ രീതിയിലുള്ള പിഡിഎഫിൽ അധിഷ്ഠിതമായ അവതരണ പ്രമാണങ്ങൾ നിർമ്മിക്കാൻ അശക്തമാണു്. പക്ഷെ ഇപ്പോഴാകട്ടെ ഈ ന്യൂനത പരിഹരിച്ചുകൊണ്ടു് ഒട്ടനവധി പ്രമാണവർഗ്ഗങ്ങൾ എഴുതപ്പെട്ടിട്ടുണ്ടു്. അവ ആധുനിക ആവശ്യങ്ങൾക്കനുസരിച്ചു് അവതരണങ്ങൾ പ്രയത്നരഹിതമായി നിർമ്മിക്കുവാൻ വളരെയധികം സഹായിക്കുന്നു. വളരെയധികം വിശേഷാൽ സൗകര്യങ്ങളുള്ള ഈ പ്രമാണവർഗ്ഗങ്ങളെ [മറ്റൊരവസരത്തിൽ](more-05) വിശദമായി പഠിക്കുന്നുണ്ടു്.


## അഭ്യാസം

വിവിധ പ്രമാണവർഗ്ഗങ്ങളെ സ്വന്തം പ്രമാണത്തിലുപയോഗിച്ചു് അടിസ്ഥാന വർഗ്ഗങ്ങളിൽ നിന്നു് വ്യത്യസ്തമായ എന്തുതരം മാറ്റങ്ങളാണു് പ്രമാണത്തിന്റെ ദൃശ്യരൂപത്തിൽ കോമ-സ്ക്രിപ്റ്റും മെമ്വാറും വരുത്തുന്നതെന്നു് ആരായുക.

```latex
\documentclass{article} % Change the class here
\usepackage[T1]{fontenc}

\begin{document}

\section{Introduction}

This is a sample document with some dummy
text\footnote{and a footnote}. This paragraph is quite
long as we might want to see the effect of making the
document have two columns.

\end{document}
```


`twocolumn` എന്ന ഐച്ഛികം `\documentclass`-നോടൊപ്പം ഉപയോഗിച്ചു് ദൃശ്യരൂപത്തിൽ വരുന്ന മാറ്റമെന്താണെന്നു മനസ്സിലാക്കുക. 

`\section` എന്ന ആജ്ഞയെ `\chapter` എന്നതിന്റെ മുകളിൽ നിവേശിക്കുക. എന്നിട്ടു് താഴെക്കൊടുത്തിരിക്കുന്ന ഐച്ചികങ്ങൾ `scrreprt` എന്ന വർഗ്ഗത്തോടൊപ്പം ഉപയോഗിക്കുമ്പോൾ പ്രമാണത്തിന്റെ ദൃശ്യരൂപത്തിൽ സംഭവിക്കുന്ന മാറ്റങ്ങളെ അവലോകനം ചെയ്യുക.

- `chapterprefix`
- `headings=small`
- `headings=big`
- `numbers=enddot`



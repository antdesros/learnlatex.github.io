---
layout: "lesson"
lang: "mr"
title: "अधिक माहिती: दृश्यकांचा समावेश"
description: "लाटेक्-मध्ये दृश्यके समाविष्ट करताना धारिकांची नावे काय ठेवावीत, पत्ते कसे लिहावेत अशा काही पायाभूत गोष्टींची माहिती आपण ह्या प्रकरणात घेऊया."
toc-anchor-text: "अधिक माहिती: दृश्यकांचा समावेश"
---

## दृश्यकांना नावे देणे

लाटेक्-सह वापरण्याच्या धारिकांची नावे विचारपूर्वक ठेवलेली बरी. सर्वात महत्त्वाचा सल्ला असा की
धारिकांच्या नावांमध्ये मोकळ्या जागा असू नयेत. उदा. जर सर्व दृश्यके एका उपपुडक्यात (सबफोल्डरमध्ये)
साठवून ठेवली असतील, तर `\includegraphics[width=30pt]{pix/mom.png}` ही आज्ञा वापरता
येऊ शकते, जिच्यात `pix` ह्या उपपुडक्याचा उल्लेख आहे व त्यातल्या `mom.png` ह्या दृश्यकाचा उल्लेख
आहे.

धारिकांच्या नावात मोकळ्या जागा सोडणे हे थोडे अडचणीचे मानले जाते, परंतु आजकाल त्याकरिताही
सोयी करण्यात येत आहेत. जर मोकळ्या जागा असलेल्या धारिकेसोबत अडचणी उद्भवत असल्या, तर त्यांतील
मोकळ्या जागा काढून धारिका चालवण्याचा प्रयत्न करा.

स्वराघाताची चिन्हे नावात वापरलेल्या धारिकांबाबत लाटेक्-चे धोरण किंचित अस्थिर आहे. काही
प्रणाल्यांमध्ये अशा धारिका चालण्यात अडचण येते. विशेषतः विंडोज़् प्रणालीवर. अशा नावांच्या
धारिकांसह काही अडचणी उद्भवल्या, तर ASCII अक्षरे वापरून धारिकेचे नाव देण्याचा प्रयत्न करून
पाहा.

## दृश्यके उपपुडक्यांत साठवणे

दृश्यकांचा समावेश आज्ञावल्यांमध्ये करते वेळी एक प्रचलित पद्धत अशी आहे की बीजधारिका ज्या पुडक्यात
आहे, त्याच्या उपपुडक्यात सर्व दृश्यके साठवणे. त्यामुळे त्यांचा वापर पत्ता देऊन करता येतो. एक
महत्त्वाची सूचना अशी की पत्त्यातील घटकांचे विभाजन करण्यासाठी `/` हे चिन्ह वापरायचे
आहे. **विंडोज़् प्रणाली वापरत असाल तरीही!**

अशा प्रकारे उपपुडक्यात जर तुम्ही अनेक दृश्यके साठवून ठेवत असाल, तर `\graphicspath` ह्या आज्ञेसह
सर्व दृश्यकांचा पत्ता निश्चित करून देता येऊ शकतो. ह्या आज्ञेस प्रत्येक उपपुडक्याचा वेगळा कार्यघटक
महिरपी कंसांमध्ये देता येऊ शकतो. उदा. `figs` व `pics` नावाची दोन उपपडकी पुढील प्रकारे
समाविष्ट करून घेता येतील.

<!-- {% raw %} -->
```latex
\graphicspath{{figs/}{pics/}}
```
<!-- {% endraw %} -->

पुडक्यांच्या नावाच्या शेवटी लिहिले जाणारे `/` हे चिन्ह विशेषत्वे पाहा.

## दृश्यके घडवणे

आपण पाहिल्याप्रमाणे लाटेक् विविध स्वरूपातील दृश्यके सहज फलितात समाविष्ट करून घेऊ शकते. जेव्हा
दृश्यकांच्या निर्मितीसाठी लाटेकेतर आज्ञावलीचा वापर केला जाईल तेव्हा शक्यतो पीडीएफ् हा पर्याय
निवडावा कारण त्यात आकार गुणोत्तराने कमी जास्त करणे सर्वात अधिक क्षमतेने शक्य आहे. बिटमॅप
स्वरूपातील दृश्यके अनिवार्य नसतील, तर शक्यतो उच्च गुणवत्तेची दृश्यकेच वापरावीत. संगणकावर तयार
केलेल्या दृश्यकांमध्ये लाटेक् आज्ञावल्यांचा समावेश [इंकस्केप](https://inkscape.org/)सारख्या
साधनांसह शक्य आहे. त्रिमितीय आकृत्यांकरिता
[एसिम्टोट](https://www.ctan.org/pkg/asymptote) ही आज्ञावली वापरता येऊ शकते. ह्या
दोहोंतर्फे फलित धारिका तयार होतात ज्यांचा समावेश लाटेक्-मध्ये करावा लागतो.

लाटेक् आज्ञावलीचा भाग असतील अशी दृश्यके लाटेक्-मध्ये घडवता येतात. त्याकरिता
[Ti*k*Z](https://ctan.org/pkg/pgf) अथवा
[PSTricks](https://ctan.org/pkg/pstricks-base) हे दोन आज्ञासंच उपलब्ध आहेत.

## तरंगती दृश्यके

लाटेक्-मध्ये तरंगत्या दृश्यकांचा समावेश करणे थोडे किचकट आहे. बहुतेक वेळा वापरकर्त्यांची अशी इच्छा
असते की बीजधारिकेत जिथे एखादी आकृती अथवा एखादे दृश्यक समाविष्ट करण्यात आले आहे, तिथेच ते
फलितातदेखील दिसावे. `float` आज्ञासंचासह हे शक्य आहे.

```latex
\documentclass{article}
\usepackage[T1]{fontenc}
\usepackage{graphicx}
\usepackage{lipsum}  % नमुना मजकूर
\usepackage{float}

\begin{document}
\lipsum[1-7]
\begin{figure}[H]
  \centering
  \includegraphics[width=0.5\textwidth]{example-image}
  \caption{An example image}
\end{figure}
\lipsum[8-15]
\end{document}
```

`H` ह्या प्राचलामुळे आकृती जिथे आहे तिथेच छापली जाते ह्याची नोंद घ्या, परंतु हे प्राचल वापरणे
टाळावे असे आम्ही सुचवू, कारण ह्यामुळे तुमच्या दस्तऐवजात मोकळा पांढरा भाग निर्माण होण्याची
शक्यता असते.

## तरंगत्या दृश्यकांचे इतर प्रकार

[लवकरच](lesson-08) आपण हे पाहू की कोष्टकांचा समावेश तरंगत्या दृश्यकांमध्ये करता येऊ
शकतो. `table` ह्या क्षेत्रात त्यांची आज्ञावली समाविष्ट करावी लागते, परंतु इतर दृश्यकांसह हे
करावेच लागेल असे नाही. त्यांसाठी `figure` हे क्षेत्र लाटेक्-मध्ये उपलब्ध आहे, परंतु ते वापरले गेलेच
पाहिजे अशी सक्ती नाही. ती केवळ एक रूढी आहे.

आणखी निराळ्या प्रकारची तरंगती दृश्यके प्रसंगी आवश्यक असू शकतात. अशा दृश्यकांचा प्रत्येक प्रकार
स्वतंत्रपणे वापरला जातो. [`trivfloat`](https://ctan.org/pkg/trivfloat) आज्ञासंचासह हे
शक्य आहे. ह्या आज्ञासंचातर्फे केवळ `\trivfloat` ही एकच आज्ञा पुरवली जाते जिच्यासह नवीन तरंगते
दृश्यक तयार करता येते.

```latex
\documentclass{article}
\usepackage[T1]{fontenc}
\usepackage{graphicx}
\usepackage{lipsum}  % नमुना मजकूर
\usepackage{trivfloat}
\trivfloat{image}

\begin{document}
\begin{image}
  \centering
  \includegraphics[width=0.5\textwidth]{example-image}
  \caption{An example image}
\end{image}
\end{document}
```
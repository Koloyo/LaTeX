# LaTeX
\documentclass[12pt]{article}
\usepackage[utf8]{inputenc}
\usepackage{geometry}
\usepackage{xeCJK}
\usepackage{CJKutf8}
\usepackage{xeCJK}
\usepackage{graphicx}
\usepackage{caption} 


\usepackage{setspace}
\geometry{hmargin=2.5cm,vmargin=4cm}

\title{La traduction automatique des idéogrammes japonais}

\author{Louise PATRICE }

    \vspace{1cm} 
\date{Année académique 2019 - 2020}

\begin{document}
\makeatletter
  \begin{titlepage}
  \centering
      {\large \textsc{Université Libre de Bruxelles}}\\
      \textsc{Architecture des systèmes d'informations}\\

    \vspace{1cm} 
    \vspace{1cm}
      {\large\textbf{	\@date\\
       }}\\
       
    \vfill
       {\LARGE \textbf{\@title}} \\
        
    \vspace{2em}
        {\large \@author} \\
    \vfill
        \vspace{10em}
      {\large \textsc{Master en sciences et technologies de l'information et de la communication}}\\
  
  \end{titlepage}
  
  
\renewcommand{\contentsname}{Table des matières.}
\tableofcontents

\makeatother
\maketitle
\part*{Introduction}




\onehalfspacing
\indent 

Les recherches concernant la traduction automatique du français au japonais restent très peu nombreuses à ce jour. À l’éloignement géographique se couplent de nombreuses différences entre les deux idiomes, comme toutes les langues. Cependant, tout un système d’écriture, comme nous l’aborderons, sépare ces deux cultures et c’est pourquoi il est d’autant plus intéressant de l'expliciter afin de mieux pouvoir entrer dans le sujet des difficultés de la traduction automatique.


En effet, nombreuses sont les plaintes concernant la traduction automatique japonaise tout particulièrement. Dans une ère où prédomine l’échange constant d’informations ainsi que de données, et où la popularité touristique du Japon augmente\footnote{ “ En 2017, pas moins de de 28,69 millions de visiteurs étrangers (en provenance de tous pays) ont foulé le sol japonais, soit 19,3\%de plus qu’en 2016.” http://www.quotidiendutourisme.com
}, les outils de traduction ne sont pas délaissés pour autant. 
Il est très peu probable que les touristes qui affluent de plus en plus au pays du Soleil Levant puissent couramment parler le japonais. Ces derniers vont donc très probablement se diriger vers des sites de traduction automatique comme Google Traduction ou encore Reverso. Or, le plus souvent, une traduction approximative peut en ressortir. Nombreuses seront les raisons à cela, et c’est pour cela que ce travail sera structuré de façon à les présenter. 

Ce sujet est également l’occasion d’expliciter le fonctionnement des bases de la langue japonaise ainsi que celui des outils de traduction automatique, qu’ils soient à l’écrit ou au travers de l’exemple des Google Word Lens qui sera aussi abordé. Enfin, il permettra de mettre en avant la façon de traduire les idéogrammes japonais tout particulièrement. C’est en effet au sein de cette thématique que se trouve le défi le plus intéressant, et complexe, de la traduction de la langue nippone. 
Cela permettra enfin de mettre en avant les difficultés que peuvent rencontrer la traduction automatique.



\part*{I. Le japonais.}
\section{Bases et particularités de la langue nipponne.}
\subsection{ Caractéristiques générales.}

             

\onehalfspacing
\indent             

Comme précédemment expliqué, le japonais possède des caractéristiques qui lui sont propres et qui sont importantes à citer dans un premier lieu afin de mieux pouvoir se pencher sur ce travail. Avant d’aborder les trois systèmes d’écritures dans les sous-parties suivantes, nous allons tout d’abord énoncer les aspects que l’on retrouve constamment dans la construction linguistique nipponne.  

Tout d’abord, on peut dire que les parties du discours sont composées de verbes, noms, adverbes, conjonctions et de particules enclitiques. Pour ce qui est de l’ordre des mots, le prédicat est placé à la fin de la phrase. Le qualificatif ou le modificatif se place devant le mot à, dans l’ordre, qualifier ou modifier. Pour ce qui est du prédicat précédemment évoqué, on en trouve trois sortes : le verbe, l’adjectif, et le nom accompagné de 
\begin{CJK}{UTF8}{min}です(だ)\end{CJK}, prononcé “desu (da)”. Le prédicat complète la phrase en apportant des notions comme : affirmatif / négatif ou passé / non passé. Ce même prédicat est invariable selon la personne, le genre, et le nombre.

De plus, les particules enclictiques, placées après le mot ou la phrase, servent à indiquer la relation grammaticale entre les mots et à ajouter différents sens à la phrase. Enfin, le sujet et l’objet sont souvent omis lorsque le contexte de l’énoncé permet de les comprendre sans les nommer : il s’agit de l'ellipse.\footnote{\samepage Toutes ces informations peuvent être retrouvées dans Minna no nihongo Shokyû 1 : Traduction et notes grammaticales, version française (Japonais) Broché – 1 janvier 1999, publié par A3 Corporation, dont le président et directeur général est Takuji Kobayashi. La seconde édition fut publiée en 2012.}

Il y a trois types d’écriture dans la langue japonaise : hiragana, katakana et kanji. Les deux premiers sont des syllabaires, que l’on peut regrouper dans la catégorie des kana, tandis que la troisième catégorie désigne les idéogrammes. C’est pourquoi cette dernière sera expliquée dans une catégorie à part entière, tandis que les deux premières seront décrites à la suite de ces explications sur les caractéristiques.

\subsection{Hiragana.}


\onehalfspacing
\indent 

Ainsi, une des principales différences entre l’alphabet romain moderne et l’écriture nippone est donc l’utilisation de deux syllabaires : les hiragana et les katakana. Comme on peut l’observer dans le tableau ci-dessous, les hiragana sont des syllabogrammes dont la forme est relativement courbée dans l’ensemble.
\space
\begin{center}

\includegraphics{figure1.png}
\captionof{figure}\centering {Tableau des hiragana. En rouge sont ceux que l’on n’utilise plus de nos jours.}
\label{fig1} \end{center}
\pagebreak

Il faut savoir qu’à l’origine, les japonais n’avaient pas de système d’écriture qui leur était propre. C’est après le Vème siècle uniquement qu’ils vont adopter l’écriture des kanji, importée de Chine. Ils étaient appelés man'yōgana \begin{CJK}{UTF8}{min}(万葉仮名).\end{CJK}\footnote{\samepage “Origins of Hiragana\begin{CJK}{UTF8}{min}(ひらがな).\end{CJK}and Katakana\begin{CJK}{UTF8}{min}(カタカナ).\end{CJK}”, Coto Academy, February 2, 2016.}

Cependant, ces derniers étant très complexes,  une transition se fit rapidement vers des caractères plus simples : les kana. On peut montrer ainsi un exemple de cette transition avec, dans l’ordre, les man'yōgana, la transition en hiragana puis en katakana. La simplification est ainsi très parlante de par cette observation : 


\begin{CJK}{UTF8}{min}安 →あ  → ア (a) \end{CJK} 

\begin{CJK}{UTF8}{min}以 →い  → イ(i) \end{CJK}\footnote{Ibid.}

Les hiragana sont principalement utilisés afin d’écrire des mots originaires du Japon, ce qui ne sera pas nécessairement le cas des katakana. 

\subsection{Katakana.}

\onehalfspacing
\indent 

On peut se demander pourquoi il existe deux syllabaires qui comportent des même sons au sein de la langue nipponne. En effet, comme on peut le voir sur le tableau ci-dessous, les deux systèmes d’écriture retranscrivent les même sons, mais avec des caractères qui ne sont pas similaires. Alors, on peut s’interroger sur la façon dont il faut utiliser un syllabaire plutôt qu’un autre. De plus, on peut remarquer que ces caractères sont beaucoup plus angulaires et géométriques que les hiragana précédemment présentés.


L’intérêt de ce syllabaire plus géométrique réside dans son utilisation réservée aux mots de langue étrangère. Par exemple, le mot France en japonais se prononce “Furansu” et s’écrit de la façon suivante à l’aide des katakana : \begin{CJK}{UTF8}{min}フランス (Fu + Ra + N + Su). On peut également penser à コンピュータ \end{CJK} (konpyūta, de l'anglais computer).  De plus, Le katakana est utile afin d’ajouter de l'emphase, tout comme l'italique est utilisé en anglais.

\begin{figure}
\centering
\includegraphics{figure2.png}
\caption{Tableau des katakana. En rouge sont ceux que l’on n’utilise plus de nos jours.}
\label{fig2} \end{figure}


\section{Les idéogrammes japonais.}
\subsection{Histoire et définition.}

\onehalfspacing
\indent 


Les kanji, comme précédemment quelque peu expliqué, ont été importés de Chine au travers de la péninsule coréenne, très proche géographiquement. À ce moment de l'histoire, le Japon n'avait pas son propre système d'écriture, et bien qu’on ne soit pas sûr du moment où le Japon a commencé à utiliser l'écriture chinoise, ce sont probablement les immigrants chinois qui ont commencé à l'utiliser. Cela prendra par la suite beaucoup d’ampleur. 


Ce sont des idéogrammes, c'est-à-dire que chaque caractère a sa propre signification et correspond à un mot. En combinant les caractères, il est possible de créer plus de mots. Par exemple, la combinaison de "électricité" avec "voiture" signifie "train". Il existe plusieurs dizaines de milliers de caractères, dont 2000 à 3000 sont nécessaires pour comprendre les journaux. Un ensemble de 2136 caractères a été officiellement déclaré comme étant nécessaire afin de pouvoir en faire un usage quotidien.


\subsection{Utilisation.}

\onehalfspacing
\indent 


Aujourd'hui, ces trois systèmes d'écriture sont utilisés ensemble, parfois même dans la même phrase. Cela s'explique en partie par la lisibilité. Le kanji crée des ruptures naturelles dans une phrase qui permettent au lecteur de séparer plus facilement les noms et les verbes.

Une phrase en hiragana seulement serait difficile à analyser puisqu'il faudrait repérer ses parties constitutives et décrire leurs rôles syntaxiques. On pourrait comparer cela comme une phrase écrite en anglais sans aucun espace entre les mots.  Cependant, les langues chinoise et japonaise étaient, et sont toujours, très différentes, ce qui signifie que l'adoption du kanji n'a pas dû être facile. Beaucoup de modifications et de changements en ce qui concerne la prononciation et la façon d'écrire ont dû être faits pour adapter les idéogrammes à la langue japonaise.

S'il est possible que le Japon simplifie encore plus ses systèmes d'écriture, le pays semble assez satisfait de continuer à utiliser les trois. On peut voir ci-dessous un exemple de phrase simple qui combine les trois systèmes d’écriture nippone, qui nous permet également d’observer que le nom est au début de la phrase dans la grammaire japonaise.


\begin{center}
\centering
\includegraphics{figure3.png}
\captionof{figure}{Les trois types d’écritures japonaises.}
\label{fig3} \end{center}

\pagebreak
\subsection{Complexité de traduction.}

\onehalfspacing
\indent 

Une autre particularité des kanji est qu’ils ont plusieurs lectures. C’est ici que la question de la traduction se complique grandement. En effet, un même idéogramme peut se lire de deux façons différentes :
\\

- On-yomi, qui est la lecture chinoise. 
\\

- Kun-yomi, qui est la lecture japonaise.
\\

Ainsi, un même idéogramme peut avoir plusieurs prononciations comme il est illustré de façon assez simple sur ce tableau :

\begin{center}
\includegraphics{figure4.png}
\captionof{figure}\centering {Exemple de lecture "Kun" et "On". 
\\Source : https://www.japanesewithanime.com/2017/12/kunyomi.html}
\label{fig2} \end{center}


Lorsque deux kanji forment un seul mot, il s’agit le plus souvent de la lecture Kun’yomi, ce que l'on appelle donc la lecture sino-japonaise. A contrario, lorsqu’un mot n’est formé que d'un seul kanji, c'est donc la lecture On'yomi.
\pagebreak

Par exemple : \\

\begin{CJK}{UTF8}{min}
 - 火 = ひ = feu, prononcé “ hi ”. `
 \\
 
- 山= やま = La montagne, prononcé “ yama ”.

\\

Or, si on regroupe ces deux kanji, on retrouve : \\

 火山=かざん  , prononcé “ kazan ”, le volcan.
Bien que “ hi ” et “yama” puissent être lus séparément, “ volcan ” ne se lit pas “ hiyama ” mais bel et bien “kazan”.

 \end{CJK}
 Ainsi, lorsque l’on observe un seul mot formé de deux kanji, c’est le plus souvent la lecture Kun-yomi qui prédomine. À l’inverse, quand le mot n’est formé que d'un seul kanji, on utilise souvent la lecture On-yomi. Cependant, ces lectures dépendent essentiellement du contexte de la phrase dans laquelle elles sont utilisées. Il faut ainsi apprendre par cœur la prononciation de chaque lecture et quand les utiliser. Cela peut déjà poser une première problématique concernant la traduction automatique, pour laquelle il peut être complexe de saisir le sens d’un idéogramme auquel l’utilisateur qui a transmis une requête de traduction s’attend et non pas une autre lecture. 

\section{L’importance du contexte et de l’intonation.}
\subsection{ Accents selon les zones géographiques.}

\onehalfspacing
\indent 

En France comme en Belgique, on retrouve différents accents selon les lieux où l’on se rend. On retrouve le même phénomène au Japon. Leur existence me paraît aussi importante qu’intéressante car c’est un paramètre de plus qu’il pourrait être enrichissant à étudier dans le cas de la traduction. En effet, il est parfois impossible pour une personne qui possède un bon niveau de japonais de comprendre certains patois sur l’île nippone. 

À titre d’exemple, on peut citer les dialectes Kagoshima (Kyushu) et d’Aomori (Tohoku), difficilement compréhensibles pour des habitants originaires d’autres régions. Le Japon comprend ainsi “plus d’une vingtaine de dialectes dont l’existence a pu être mise à mal par le japonais standard” également appelé hyōjun-go.\footnote{ “ Japan Time, Opening up to difference: The dialect dialectic", BY ROGER PULVERS, MAY 23 2006.} 

Comment les logiciels procèdent-il dans le cas d’un patois particulier ? De base, il est très complexe de traduire le japonais de par les nombreuses subtilités qu’il comporte comme nous l’avons précédemment évoqué au cours des chapitres précédents. Ainsi, puisqu’il n’existe pas d’études à ce sujet, j’ai essayé moi-même de traduire une réplique dans le dialecte d’Hiroshima, venant du film " Combat sans code d’honneur "  réalisé par Kinji Fukasaku, et sorti en 1973.\footnote{Réplique précise trouvée à l’écrit dans "Les dialectes au Japon et l’Hiroshima-Ben" AU JAPON ET L’HIROSHIMA-BEN, JUDITH COTELLE, 24 septembre 2016, https://www.jud-hiroshima.com/2016/09/24/dialecte-hiroshima/
 } 
 
 Que cela soit en anglais comme en français, la traduction issue de Google Traduction ne semble pas fonctionner puisqu’elle ne retranscrit que le premier mot de la phrase originale en japonais. Comme on peut le voir ci-dessous, il s’agit donc de “ Washa” qui, en anglais comme en français, ne signifie rien.  


\begin{center}
\includegraphics{figure5.png}
\captionof{figure}\centering {Google Translate}
\label{fig5} \end{center}

Au-delà de la dimension linguistique, il ne faut pas oublier que chaque patois correspond à une politique, un passé bien particulier. Autrefois, en temps de guerre, ils étaient dépréciés car ils ne correspondaient pas à une idée d’unité nationale qui était à l'époque tout particulièrement importante. 


Or, depuis quelques années, on peut remarquer qu’on cherche à les conserver car il sont le fruit de toute une identité culturelle. Le Kansai-ben, utilisé dans la région du Kinki, fait souvent référence à des comédies par exemple. 


\subsection{Intonation, prosodie et évolution dans le temps du japonais.}

\onehalfspacing
\indent 

Cependant, au-delà des accents, on peut également parler de la prosodie, c’est-à-dire les recherches sur l'accent et sur l'intonation ; l'étude du rythme, du débit et des pauses dans la parole. Selon Chieko Shirota, l’exposé, la conférence, le discours public, les reportages et les actualités télévisées seront cependant beaucoup plus complexes à comprendre pour les japonais, même au sein d’un même dialecte, qu’une situation conversationnelle.\footnote{Chieko Shirota. Syntaxe et prosodie en japonais. Lecture d’Informations télévisées / Dialogue spontané. Linguistique. Université de la Sorbonne nouvelle - Paris III, 2012. Français. ffNNT : 2012PA030151ff. fftel-01151552f.} 

 La raison à cela est que , bien que l’on puisse penser que l’intonation a un rôle secondaire par rapport à la compréhension grammaticale et syntaxique, ce n’est pas le cas dans la langue japonaise. 
 
 Les degrés d'intonation, qu’ils soient hauts ou bas, occupent une place très importante au sein de la langue japonaise. Par exemple, les homophones peuvent avoir différents degrés, ayant différentes significations avec un ton plus doux, même si ce mot est écrit avec des sons identiques. La plus grande barrière pour les apprenants du japonais et les personnes étant capables de le parler couramment, est d’avoir une intonation correcte. Beaucoup d'étudiants en japonais parlent souvent sans prêter attention à l'intonation correcte des sons rendant le discours incorrect. Il n'est pas pratique de mémoriser ou tenter de créer une logique de règles pour les différents degrés d'intonation, d'autant plus qu'ils peuvent changer selon le contexte ou le dialecte. La conversation, du fait qu’elle comporte beaucoup plus d’éléments du paralangage, sera plus facile à aborder au niveau de la compréhension pour les interlocuteurs.  
 
Ces questions sur l’intonation qui participent à la traduction du sens d’une phrase ou d’un mot seront, comme nous le verrons, particulièrement complexes à aborder pour un logiciel de traduction automatique.
\pagebreak

De plus, la langue nippone a beaucoup évolué au fil du temps, comme il m’a paru important de le souligner dans le tableau ci-dessous issu de \textit{La phonologie du japonais} de Laurence Labrune.\footnote{La phonologie du japonais, Laurence Labrune, 2006. https://books.google.fr/books/about/La phonologie\-du\-japonais.html?id=vf2XO0ls3GYC&printsec=frontcover&source=k\-read\_button&redir\_esc=y#v=onepage&q&f=false}


\begin{center}
\includegraphics{figure6.png}
\captionof{figure}\centering {La phonologie du japonais, Laurence Labrune, 2006.}
\label{fig5} \end{center}

Sans entrer dans les détails linguistiques, il s’agit de poser une autre réflexion sur les traductions automatiques et de se demander si elles pourraient être capables de traduire d’anciens textes en japonais malgré les nombreuses transformations et réformes linguistiques qu’a traversé la langue. 

\subsection{L’importance du contexte : le cas " mokusatsu" .}

\onehalfspacing 
\indent 

Au sein de l’Histoire, on retrouve des erreurs de traductions qui ont eu des conséquences plus ou moins importantes dans le cadre diplomatique. Cependant, une de ces dernières sera cruciale puisqu’elle jouera un rôle dans le largage de la bombe d’Hiroshima en 1945. 

Dans le cadre de cette étude, ce tragique exemple paraissait significatif de la subtilité et de la complexité dont peut faire preuve la langue japonaise. Il faut néanmoins prendre du recul sur cette anecdote et bien comprendre que les tensions politiques présentes durant cette période historique sont bien plus complexes à traiter qu’une bénigne erreur de traduction.

Alors que les tensions sont très importantes entre la Chine, les Etats-Unis et la Grande Bretagne envers le Japon, un ultimatum sera posé au Pays du Soleil levant le 26 juillet 1945, demandant à ce que ce dernier capitule complètement. Le Premier ministre Suzuki choisit d’utiliser le terme "mokusatsu".
\begin{CJK}{UTF8}{min}( 黙殺 ) dans sa réponse. Or, " mokusatsu "  ( 黙殺 )  est composé des kanji 黙 (moku) " silence " et 殺 (satsu) " tuer ", dans leur sens premier.)\end{CJK}

Si l’on recherche ce mot dans les dictionnaires japonais, on trouve les définitions " ignorer, ne pas répondre ". C’est l’agence de presse Dōmei, agence officielle de l’Empire à l’époque, qui va décider  de traduire " mokusatsu " du japonais vers l’anglais par " ignore " . Les médias vont ainsi interpréter cette réponse comme un refus de capitulation. Cela va donner lieu à l’utilisation de la bombe nucléaire.  

Or, selon le chercheur historien Kawai Katsuo\footnote{ KAWAI Kazuo. " Mokusatsu  , Japan's Response to the Potsdam Declaration"}, cette réponse est très complexe à traduire étant donné qu’il n’y a pas d’équivalent en anglais. De plus, le rejet est très rarement exprimé de façon démonstrative dans la langue japonaise. Selon Kawai, dans ce contexte, il s’agissait plutôt de traduire " mokusatsu " par " se garder de tout commentaire". Le ministre Suzuki voulait ici exprimer son besoin de voir l’évolution des évènements, de ne pas prendre de décision immédiate, d’après le chercheur. Mais étant donné l'ambiguïté de la langue ainsi que les tensions présentes à cette époque, cette erreur de traduction aura de grandes conséquences. 

Le lien que nous pouvons faire avec la traduction automatique par rapport à cet exemple est bien évidemment que les différences entre les langues, au-delà du contexte touristique, peuvent également intervenir dans des situations diplomatiques. Si, à l’avenir, les outils de traduction automatique sont utilisés en complément de traducteurs humains, il faut s’assurer que ces derniers puissent être assez performants pour pouvoir nuancer ce type d'ambiguïté.  

\pagebreak

\part*{II. La traduction automatique.}
\section{Présentation.}
\subsection{ Bases d’une recherche et le traitement automatique du langage naturel (abr. TALN).}

             

\onehalfspacing
\indent             

Internet est une plate-forme où de nombreuses informations circulent en permanence. Or, il se trouve que certaines ne puissent être lues, si elles sont dans une langue différente que celles que puissent lire l’utilisateur. C’est souvent le cas dans lequel rentre en compte la traduction automatique. Nous avons vu précédemment dans chaque sous-chapitre les nombreuses conditions à respecter afin d’obtenir une traduction correcte, tout particulièrement en japonais. 

Ainsi, on ne peut souvent pas proposer une seule bonne traduction à une requête. Comme nous l’avons vu précédemment, nombreuses sont les complexités de la langue nippone, et il en va de même pour les autres langues. C’est pourquoi, lorsqu’un utilisateur fait une requête dans une langue dite “source” vers une dite “cible” à l’aide d’un outil de traduction assistée par ordinateur, on n’obtient pas forcément qu’une seule réponse. Reverso utilise par exemple des phrases complètes en tant qu’exemple afin que l’utilisateur puisse lui-même déterminer quelle traduction semble la plus appropriée à sa recherche. 

\begin{figure}
\includegraphics{figure7.png}
\captionof{figure}{Reverso.}
\label{fig5} \end{figure}

\pagebreak
On peut également parler du “Natural Language Processing” (NLP), aussi appelé “traitement automatique du langage naturel” (TALN, pouvant être appelé "ingénierie linguistique"). Il s’agit d’un ensemble de techniques qui permet la traduction automatique que nous expliciterons par la suite. Ainsi, la racinisation est un de ces fonctionnements. On peut assembler certains termes qui possèdent une racine commune et appartenant au même champ lexical. Par exemple, pêche, pêcher, pêcheur ont la même racine, mais ni la pêche (le fruit), ni le péché, ne font partie du même champ lexical. 

La lemmatisation, autre fonctionnement au sein du TALN, consiste à regrouper des mots d'une même famille dans un texte, afin de réduire ces mots à leur forme canonique. Elle s’intitule le lemme. 

Certaines conjugaisons peuvent rendre cette tâche complexe pour des ordinateurs, comme retrouver la forme canonique " avoir " depuis " eussions eu ". En revanche, " des avions " et " nous avions " n'ont pas le même lemme. Nous verrons par la suite comment aborder ce type de thématique avec la langue japonaise, et allons dans un premier lieu poursuivre sur le fonctionnement de la traduction automatique.

Cependant, si l’utilisateur n’a pas une très bonne maîtrise de la langue, le mieux est que l’outil de traduction assistée soit capable de répondre à la requête demandée avec exactitude,bien que cela soit tout de même utopique. C’est pourquoi il est intéressant de se pencher sur le fonctionnement en détails de la traduction automatique statistique, car cela va nous permettre de mieux comprendre les rouages.

On peut parler dans un premier lieu de l’alignement des mots. Ce système permet d’établir un score de probabilité concernant la traduction de termes. Il utilise des corpus de textes au préalable afin de pouvoir enregistrer les traductions les plus probables. 
\pagebreak
\begin{center}
\includegraphics{figure8.png}
\captionof{figure}{Dictionnaire bilingue généralisé et probabilisé, construit automatiquement à partir d’un corpus bilingue parallèle.}
\label{fig5} \end{center}


Ce type de système est notamment très utile lors de la traduction de certains termes spécialisés puisque ces derniers sont tant ciblés qu’ils n’ont souvent pas forcément des problèmes de polysémie. La traduction automatique se rapproche alors, d’une certaine façon, de la linguistique de corpus. Cependant, il est très complexe de nos jours pour les logiciels de traduire à la perfection une grande quantité de texte. Encore plus si ce dernier est générique. Dans ce type de cas-ci , il n’est pas rare qu’un traducteur doive vérifier une seconde fois la traduction automatique. En plus des interfaces disponibles en ligne, citées précédemment, comme Google Traduction ou encore Reverso, on peut également relever des logiciels développés par Systran 3. \footnote{Raphaël Rubino. Traduction automatique statistique et adaptation à un domaine spécialisé. Autre [cs.OH]. Université d’Avignon, 2011. Français. ffNNT : 2011AVIG0186ff. fftel-00879945f}


\subsection{ Fonctionnement des “mémoires de traduction”. }

\onehalfspacing 
\indent 


On retrouve également les dites “mémoires de traduction”, également abréviées “MT”.  Bien que ce fonctionnement soit à nuancer de la traduction automatique. En effet, cette dernière peut se suffire à elle-même bien qu’elle sera plus approximative et va nécessiter une certaine réflexion venant de l’utilisateur. 

Or, le fonctionnement des MT, qui sont donc plutôt considérées comme des outils de traduction assistée par ordinateur (TAO), est focalisé sur une base de données. En effet, lorsqu’un traducteur va lancer un programme MT comme nous allons en citer par la suite, le texte à traduire sera segmenté. Si il y a une correspondance complète comme lointaine dans la base de données avec ce même texte segmenté, elle sera proposée au traducteur. Ce dernier aura le choix d’utiliser cette proposition comme de ne pas le faire, ou bien de la modifier, toute nouvelle proposition sera enregistrée dans la banque de données. 

\section{Difficultés avec le japonais.}

\subsection{Différences grammaticales. }

\onehalfspacing 
\indent 


Le japonais est l'une des langues les plus difficiles à apprendre pour les Occidentaux. L'inverse est également vrai car la structure grammaticale des deux langues est très différente. Il en résulte que la précision de la traduction en souffre souvent, ce qui se traduit par des formulations maladroites indiquant clairement qu'un document n'est pas dans sa langue d'origine.

Ces différences causent un certain nombre de problèmes dans la traduction du japonais vers l'anglais. La plupart des traductions tentent de conserver l'équivalence entre la langue source et la langue cible en préservant le sens et l'intention du texte source et la structure syntaxique. De plus, il est pratiquement impossible de maintenir un nombre équivalent de mots pour les mots ou de phrases pour les phrases.
Comme nous l’avons vu précédemment dans le cas “ mokusatsu”, nombreux mots et phrases ne peuvent être traduits littéralement, ce qui rend la traduction de concepts abstraits extrêmement difficile. 

De plus, il n’y a pas de temps futur, et pas de noms pluriels. Ces structures grammaticales sont très présentes en Occident et c’est pourquoi il est complexe pour les outils de traduction de faire office de passerelle entre les deux langues sans faire de fautes. 

\subsection{Processus de traduction et complexité des kanji.}

\onehalfspacing 
\indent 

Ainsi, la traduction entre ces deux langues est relativement complexe. Le processus peut comporter jusqu'à cinq étapes, au lieu de la seule analyse sémantique et transformation syntaxique qui se produit lors de la traduction dans les langues indo-européennes. Alors que la traduction du japonais vers l'anglais commence par une analyse sémantique, il y a souvent plusieurs étapes où le traducteur doit faire des allers-retours entre les deux langues, en décomposant les phrases en plus petits morceaux, pour obtenir le sens et les nuances juste assez justes pour produire un texte à la sonorité naturelle. Les entreprises qui fournissent des services de traduction en japonais sont mieux équipées pour gérer des projets vastes et complexes car elles suivent des procédures systématiques et utilisent des outils qui réduisent le temps de traduction et les frais généraux.


Contrairement aux langues occidentales, le japonais écrit n'a pas de majuscules ni de minuscules. Il y a simplement le Kanji que nous avons précédemment présenté, la forme de caractère complexe qui prend sa signification à partir du placement des traits, du placement des caractères lors des lectures, des lectures kun et plus encore. 



En raison de ces complexités, la traduction du japonais vers l'anglais ou même le français nécessite souvent au moins deux passages dans un document pour obtenir un texte qui non seulement est exempt d'erreurs, mais qui s'écoule et se lit facilement. Comme la traduction un à un est pratiquement impossible, les traducteurs doivent saisir le contenu, et non la forme, et utiliser la voix active et être succincts dans l'utilisation des mots. 


\subsection{La dernière mise à jour de Google.}

\onehalfspacing 
\indent 

La dernière mise à jour de Google dans le domaine de la traduction linguistique a permis de réaliser un saut technologique dans le domaine de la traduction plus important que tous ceux des dix dernières années réunies. La traduction de Google utilisera désormais la traduction automatique neurale pour traduire des phrases entières à la fois, par opposition à la traduction mot à mot. Le résultat, selon les chercheurs, sera beaucoup plus proche d'une traduction humaine et le résultat final sera beaucoup plus facile à lire.

En septembre 2016, Google a annoncé que les réseaux neuronaux commencent à alimenter Google Translate, et à la mi-novembre, il a publié la technologie pour huit paires de langues, spécifiquement de et vers l'anglais, le français, l'allemand, l'espagnol, le portugais, le chinois, le japonais, le coréen et le turc. Le système n'est pas sans défaut et fait toujours des erreurs. Il oublie de traduire des mots ou ne comprend pas les noms des personnes. Cependant, les erreurs ont été réduites de 55 à 85\% dans un certain nombre de langues. Est-ce que cela marquera le début d'une nouvelle ère pour l'industrie de la traduction, et tout particulièrement dans la compréhension du japonais ? 

La traduction automatique neuronale  utilise une technologie de pointe pour fournir des traductions plus précises en fonction du contexte, au lieu de phrases brisées traduites mot à mot, ce qui améliore considérablement la qualité de la traduction. Elle s'appuie sur des réseaux neuronaux récurrents à mémoire à court terme  et des réseaux neuronaux qui ont été formés par des unités de traitement graphique  et de l'unité de traitement de tenseur. Le transfert de connaissances est l'ingrédient clé de cette nouvelle recette et Google l'appelle " Zero-Shot Translation ", ce qui permet essentiellement aux machines d'apprendre à traduire entre deux langues sans être formées au préalable pour le faire. En termes simples et en utilisant l'exemple de Google, le nouveau système est capable d'apprendre à la machine à traduire entre le coréen et le japonais sans avoir été préalablement formée à ces paires de langues. Les chercheurs de Google ont effectué des expériences afin d'entraîner le système multilingue avec des paires de langues souhaitables, telles que japonais-anglais et coréen-anglais. Le système GNMT a ensuite partagé ses paramètres pour traduire entre ces quatre paires de langues et ils ont découvert qu'il était possible pour le système de traduire ensuite entre le coréen et le japonais sans aucune formation préalable. Mais de quelle façon ?

Le nouveau système, ont découvert les chercheurs de Google, transfère la " connaissance de la traduction " d'une paire de langues aux autres et, selon les chercheurs de Google, " cela signifie que le réseau doit encoder quelque chose sur la sémantique de la phrase plutôt que de simplement mémoriser les traductions de phrase à phrase. Les détails de cette percée sont encore opaques, mais il s'agit néanmoins d'une invention pionnière, car c'est la première fois que ce type d'apprentissage par transfert fonctionne en traduction automatique. On ne peut espérer ainsi que des améliorations en ce qui concerne la traduction du japonais. 
\pagebreak
\part*{Conclusion}

\onehalfspacing 
\indent 

Avec l'arrivée des Jeux Olympiques d'été de 2020 à Tokyo, les entreprises pourraient avoir besoin d'accroître leur présence sur le marché japonais. Pour atteindre cet objectif avec succès, des traductions précises sont nécessaires. Ce travail avait pour but de montrer les subtilités et la passionnante originalité de la langue japonaise, raison pour laquelle cet idiome est tout aussi fascinant que complexe à traduire. Différentes approches de traduction automatique ou de traduction assistée par ordinateur ont également été exposées, tout en expliquant la nuance entre ces dernières. Ces recherches furent tout particulièrement intéressantes puisqu’elles m’ont permis d’apprendre de nombreuses nouvelles anecdotes sur des domaines auxquels je m’intéressais déjà pourtant auparavant et surtout de mieux comprendre ce qui se passait derrière une requête de traduction. 

Il est captivant de voir que de nombreuses innovations continuent à ce jour d’émerger afin de pouvoir se rapprocher toujours un peu plus de l’utopie d’une traduction parfaite. On peut évoquer en ouverture de ce travail les Google Lens qui sont conçues tout particulièrement afin de pouvoir déchiffrer la complexité des kanji. Les utilisateurs anglophones peuvent désormais traduire des mots japonais en pointant simplement l'appareil photo de leur téléphone dans leur direction, et en regardant les changements en temps réel. Ce qui est impressionnant, c'est que ce processus peut aussi se faire hors ligne une fois que vous avez téléchargé un petit fichier, ce qui permet aux touristes en visite d'utiliser leur téléphone comme un dictionnaire de poche immédiat sans avoir besoin d'une connexion Wi-Fi. 

Il s’agit ici d’une innovation parmi beaucoup d’autres, et il faut savoir que ces recherches furent tout particulièrement condensées étant donné qu’il s’agit ici d’un travail d’initiation à la recherche. Ces dernières seront complétées et étayées dans la rédaction de mon mémoire l’année à suivre et je n’ai aucun doute sur les nombreuses nouvelles évolutions que vont révéler les outils de traduction envers la langue nippone d’ici là.

\pagebreak

\begin{thebibliography}{9}
\bibitem{texbook}
Yayoi Nakamura-Delloye. Alignement automatique de textes parallèles français-japonais. Linguistique. Université Paris-Diderot - Paris VII, 2007. Français. fftel-00259276ff


\bibitem{lamport94}
Google achieves state-of-the-art NLP performance with an enormous language model and data set- KYLE WIGGERS, OCTOBER 24, 2019


\bibitem{lamport94}
Vers une nouvelle époque en traduction automatique, John Hutchins, Montréal, 1993


\bibitem{lamport94}
Raoul Blin. Traduction automatique du japonais vers le français : Bilan et perspectives. Traitement Automatique du Langage Naturel, May 2018, Rennes, France. ffhal-01796313f



\bibitem{lamport94}

Computational Linguistics and Classical Lexicography, Changing the Center of Gravity: Transforming Classical Studies Through Cyberinfrastructure, 2009, Volume 3 Number 1, David Bamman,Gregory Crane, Tufts University


\bibitem{lamport94}
Les dialectes au Japon et l’Hiroshima-Ben, Judith Cotelle, 2017

\bibitem{lamport94}
Machine Translation, M. Kay, https://www.linguisticsociety.org.

\bibitem{lamport94}
Automatic translation: Why brands need to stop waiting for AI to solve their translation problems, Alexandra Kravariti, March 19th, 2018.

\bibitem{lamport94}
Japan Time, Opening up to difference: The dialect dialectic, BY ROGER PULVERS, MAY 23 2006.

\bibitem{lamport94}
Chieko Shirota. Syntaxe et prosodie en japonais. Lecture d’Informations télévisées / Dialogue spontané. Linguistique. Université de la Sorbonne nouvelle - Paris III, 2012. Français. ffNNT : 2012PA030151ff. fftel-01151552f 

\bibitem{lamport94}
Mary-Annick Morel et Laurent Danon-Boileau, Grammaire de l'intonation, l'exemple du français, Paris, Ophrys, 1998.

\bibitem{lamport94}
De l’importance du contexte culturel en traduction, 13. décembre 2019 .https://eikyo.jimdofree.com/2019/10/13/de-l-importance-du-contexte-culturel-en-traduction/

\bibitem{lamport94}
La phonologie du japonais, Laurence Labrune, 2006

\bibitem{lamport94}
LUCKEN, Michael. « Déclaration de Potsdam » dans : Sengo, le Japon après la guerre. Presses de l’Inalco, 2017

\bibitem{lamport94}
Raphaël Rubino. Traduction automatique statistique et adaptation à un domaine spécialisé. Autre [cs.OH]. Université d’Avignon, 2011. Français. ffNNT : 2011AVIG0186ff. fftel-00879945f


\bibitem{lamport94}
Martin Benjamin 2019, Teach You Backwards: An In-Depth Study of Google Translate for 103 Languages, Kamusi Project International, https://teachyoubackwards.com


\end{thebibliography}

\end{document}

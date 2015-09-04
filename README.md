#LaTex CV/Resume Template

**Table of Contents**
- [Introduction](https://github.com/Awjin/cv_template#introduction)
- [Documentation](https://github.com/Awjin/cv_template#documentation)
  - [Importing the Class](https://github.com/Awjin/cv_template#importing-the-class)
  - [Header](https://github.com/Awjin/cv_template#header)
  - [Section](https://github.com/Awjin/cv_template#section)
  - [Entry](https://github.com/Awjin/cv_template#entry)
  - [Detail](https://github.com/Awjin/cv_template#detail)
- [Skeleton Code](https://github.com/Awjin/cv_template#skeleton-code)

#Introduction

This template focuses on the following:
- Sparse design
- Clean typography
- Customizability

Style rules are found in `my_cv.cls`. Values that are most likely to be tweaked
(margins, vertical spacing, etc.) are commented for easy editing.

---

#Documentation

###Importing the Class
Put this at the beginning of your tex file:
```
\documentclass{my_cv}
```

###Header
```
\header{name}
       {email}
       {phone}
```
Name will be displayed in large font to the left, with the rest of the
information right-aligned. You can add/remove entries in `my_cv.cls`.

###Section
Use these to organize the resume body.
```
\section{Education}

\section{Work Experience}
```

###Entry
Resume entry. There are 3 fields. #1 and #2 are left aligned, and #3 is right aligned. Common usage:
```
\entry{Job Title}{Company Name}{Dates}
```
Note that all fields are optional:
```
\entry{Job Title}{}{Dates}

\entry{Job Title}{}{}
```

###Detail
Can be used to describe a section or entry.
```
\section{}
  \detail{This is something I accomplished.}

\entry{}{}{}
  \detail{This is something that I accomplished.}
```

---

#Skeleton Code
```
\documentclass{my_cv}
\begin{document}

\header {}{}{}

\section{}

\entry{}
\detail{}

\end{document}
```
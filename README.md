# myrepo
Repository for testing my Git/GitHub setup
A line I wrote on my local computer
testing 
---
title: Curriculum Vitae
name: Katrina
surname: Lam
position: "Master Student"
address: "California Polytechnie State University, Pomona"
#phone: +1 22 3333 4444
pronouns: she/her
#www: mariecurie.com
email: "kflam@cpp.edu"
#twitter: mariecurie
github: kflam1
#linkedin: mariecurie
date: "`r format(Sys.time(), '%B %Y')`"
aboutme: "Katrina is a graduate from Cal poly Pomona who conducts research on sea slug species Trapania"
output:
  vitae::markdowncv:
    theme: kjhealy
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE, warning = FALSE, message = FALSE)
library(vitae)
```

## Some stuff about me

 * I am currently working on 79 specimens of Trapania.
 * I am a teachers assistant in the Biology Department.
 * I am a the first generation to attend college.

## Education

```{r}
library(tibble)
tribble(
  ~ Degree, ~ Year, ~ Institution, ~ Where,
  "Bachelor's in Animal Science", "2016-2019", "University of Hawaii at Manoa", "Honolulu, Oahu",
  "Master's in Biological of Sciences", "Current", "Cal Poly University of Pomona", "Pomona, California",
) %>%
  detailed_entries(Degree, Year, Institution, Where)
```

## Research Experience

```{r}
library(tibble)
tribble(
  ~ Degree, ~ Year, ~ Institution, ~ Where,
  "John A. Burns School of Medicine", "2019", "• Provide quality husbandry care for the mice in the vivarium. 
• Performed necropsies on sentinel mice and collected data. 
• Collected blood intracardially and collected fecal samples. 
• Assisted in examination and technical procedures. 
• Practiced biosafety protocols within the facility.  
", "Research Intern",
  "Cal Poly Pomona", "Current", "• Perform tissue and DNA extraction from specimens
• Set up and use a PCR machine 
• Produce agarose gel and run the electrophoresis gel
• Conduct DNA purification
", "Graduate Research",
) %>%
  detailed_entries(Degree, Year, Institution, Where)
```

## Teaching Experience

```{r}
library(tibble)
tribble(
  ~ Degree, ~ Year, ~ Institution, ~ Where,
  "University of Hawaii at Manoa", "2019", "• Taught on animal anatomy in a laboratory setting. 
• Led discussion sections, planned dissection lessons. 
• Organized study sessions, prepared students for examinations.", 
"Teaching Assistant for Animal Anatomy",
  "Cal Poly Pomona", "Current", "• Taught Biology for nonmajors in a laboratory setting. 
• Helped conduct experiments with students.", "Teaching Assistant for Biological Sciences for nonmajors",
) %>%
  detailed_entries(Degree, Year, Institution, Where)
```
## References

```{r}
library(tibble)
tribble(
  ~ Degree, ~ Year, ~ Institution, ~ Where,
  
 "DVM, Associate Specialist", "2019", "University of Hawaii at Manoa", "Jenee Odani",
  "DVM, Animal and Veterinary Services Program", "2019", "University of Hawaii at Manoa", "Michael Wong",
    "Veterinary Assistant/Trainer, Animal and Veterinary Services Program", "2019", "John A. Burns School of Medicine", "Lisa Sato",
) %>%
  detailed_entries(Degree, Year, Institution, Where)
```

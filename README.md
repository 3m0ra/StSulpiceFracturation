# StSulpiceFracturation
This repository contains the numerical annexes to Emanuele J. Morotti's Bachelor's degree work, entitled "Caractérisation d'affleurements fracturés par photogrammétrie" and carried out at the University of Neuchâtel's Centre for Hydrogeology (CHYN) under the direction of prof. Benoît Valley.
Ecco il testo formattato in stile non LaTeX:

---
Nous présentons les fichiers ci-dessous.
---
**Planes.csv**

Ce dossier contient tout les données de tous les plans extraits de la falaise traitée dans l'exemple d'application du workflow, selon les paramètres montré à la table [tab:parametres_facets]. Les colonnes du fichier incluent:
- Index : le nom du plan, tel que généré par le plugin Facets.
- CenterX : la position x du centre du plan (en CH1903+/LV95).
- CenterY : la position y du centre du plan (en CH1903+/LV95).
- CenterZ : la position z du centre du plan (en CH1903+/LV95).
- NormalX : la composante cartésienne x du vecteur unitaire normal au plan.
- NormalY : la composante cartésienne y du vecteur unitaire normal au plan.
- NormalZ : la composante cartésienne z du vecteur unitaire normal au plan.
- RMS : [m] la distance points-plan exprimée en moyenne quadratique (Root Mean Squared).
- Horiz_ext : [m] l'extension horizontale du rectangle inscrivant le plan.
- Vert_ext : [m] l'extension verticale du rectangle inscrivant le plan.
- Surf_ext : [m^2] l'aire du rectangle inscrivant le plan.
- Surface : [m^2] l'aire du plan.
- Dip dir. : [°] la direction de plongement du plan.
- Dip : [°] le plongement du plan par rapport à l'horizontale.
---
**Filtered_planes.csv**

Ce dossier contient des informations concernant les plans utilisés dans la partie analytique du mémoire. Il s'agit des plans inclus dans Planes.csv ayant le champ "Surface" d'au moins 0.2 m^2. Les colonnes du fichier sont les mêmes que pour Planes.csv, avec l'ajout d'une colonne:
- Set : le nombre du set d'appartenance du plan.
---
**St_Sulpice.ipynb**

Ce document est un fichier Python Jupyter Notebook. Il contient tout le code qui a été utilisé pour analyser les données concernant les plans extraits par CloudCompare et Facets (e.g. calcul de l'espacement entre les familles, création de figures, etc.). Une description est fournie en commentaires directement dans le fichier.

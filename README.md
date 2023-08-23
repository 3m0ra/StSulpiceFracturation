# StSulpiceFracturation
This repository contains the numerical annexes to Emanuele J. Morotti's Bachelor's degree work, entitled "Caractérisation d'affleurements fracturés par photogrammétrie" and carried out at the University of Neuchâtel's Centre for Hydrogeology (CHYN) under the direction of prof. Benoît Valley.
Nous présentons les fichiers ci-dessous. \\
\newline
\textbf{Planes.csv}\\
Ce dossier contient tout les données de tous les plans extraits de la falaise traitée dans l'exemple d'application du workflow, selon les paramètres montré à la table \ref{tab:parametres_facets}. Les colonnes du fichier incluent:
\begin{itemize}
    \item Index : le nom du plan, tel que généré par le plugin Facets.
    \item CenterX : la position x du centre du plan (en CH1903+/LV95).
    \item CenterY : la position y du centre du plan (en CH1903+/LV95).
    \item CenterZ : la position z du centre du plan (en CH1903+/LV95).
    \item NormalX : la composante cartésienne x du vecteur unitaire normal au plan.
    \item NormalY : la composante cartésienne y du vecteur unitaire normal au plan.
    \item NormalZ : la composante cartésienne z du vecteur unitaire normal au plan.
    \item RMS : [$m$] la distance points-plan exprimée en moyenne quadratique (\textit{Root Mean Squared}).
    \item Horiz\_ext : [$m$] l'extension horizontale du rectangle inscrivant le plan.
    \item Vert\_ext : [$m$] l'extension verticale du rectangle inscrivant le plan.
    \item Surf\_ext : [$m^2$] l'aire du rectangle inscrivant le plan.
    \item Surface : [$m^2$] l'aire du plan.
    \item Dip dir. : [\degree] la direction de plongement du plan.
    \item Dip : [\degree] le plongement du plan par rapport à l'horizontale. \\
\end{itemize} 
\\
\textbf{Filtered\_planes.csv} \\
Ce dossier contient des informations concernant les plans utilisés dans la partie analytique du mémoire. Il s'agit des plans inclus dans Planes.csv ayant le champ "Surface" d'au moins 0.2 $m^2$. Les colonnes du fichier sont les mêmes que pour Planes.csv, avec l'ajout d'une colonne:
\begin{itemize}
    \item Set : le nombre du set d'appartenance du plan. \\
\end{itemize}
\\
\textbf{St\_Sulpice.ipynb}\\
Ce document est un fichier Python Jupyter Notebook. Il contient tout le code qui a été utilisé pour analyser les données concernant les plans extraits par CloudCompare et Facets (e.g. calcul de l'espacement entre les familles, création de figures, etc.). Une description est fournie en commentaires directement dans le fichier.

# Virtual Python environments

Een virtual Python environment is een omgeving met een installatie van een Python versie, met de bijgevoegde packages die men erin kan installeren (via pip commando's). 

Voordat je conda kan gebruiken, installeer Anaconda (https://www.anaconda.com/). 

Maak daarna een virtuele omgeving maken met het ‘conda’ commando (run in een terminal): 

`conda create -n <env-naam> python=3.12`

<sdsds>

<env-naam> = zelf gekozen environment name
Pas op: Mocht je geen python=3.12 geven, dan gebruikt hij de python versie die er bij Anaconda is geinstalleerd
De conda installatie komt hier te staan: /opt/anaconda3/envs/<env-naam>


`conda create -n &lt; env-naam &gt; python=3.12`


conda create -n ragchat python=3.12
conda activate ragchat

Om te exporteren
conda activate ragchat
conda env export --from-history > environment.yml
 </pre>

![alt text](image.png)


<pre lang="markdown">
conda create -n \<env-naam>\ python=3.12 </pre>

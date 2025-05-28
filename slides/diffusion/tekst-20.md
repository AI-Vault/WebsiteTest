# Uitleg van de Slide: Sampling is Slow

## Inleiding
Op deze slide wordt het probleem van langzame sampling in machine learning besproken, specifiek in de context van beeldgeneratie. Het legt uit waarom het genereren van nieuwe beelden tijdrovend is en introduceert twee verschillende benaderingen: DDPM en DDIM.

## Probleem van Langzame Sampling
- **Veel Tijdstappen**: Sampling is traag omdat er veel tijdstappen zijn.
- **Afhankelijkheid**: Elke tijdstap is afhankelijk van de vorige stap, wat betekent dat het proces sequentieel is (Markoviaans).

## Oplossingen voor Versnelling
Er zijn verschillende samplers ontwikkeld die dit probleem aanpakken. Eén daarvan is DDIM.

### DDPM (Denoising Diffusion Probabilistic Models)
- **Volledige Gebruiksduur**: DDPM maakt gebruik van alle tijdstappen in het generatieve proces. Dit kan leiden tot traagheid.

### DDIM (Denoising Diffusion Implicit Models)
- **Snelheid**: DDIM daarentegen slaat tijdstappen over, waardoor het proces sneller is.
- **Voorspelling en Verfijning**: Het maakt een ruwe schatting van de uiteindelijke output en verfijnt deze vervolgens met behulp van het denoising-proces.

## Conclusie
DDIM biedt een snellere methode voor beeldgeneratie door het overslaan van tijdstappen en efficiënt om te gaan met de voorspelling van de uiteindelijke output.
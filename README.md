# ISAAC Ontology Network
This repository contains the source code of ISAAC Ontology Network.


### What is ISAAC?

ISAAC is a modular ontology for Image Schema Abstraction And Cognition, building a new top image schematic roles level on frames represented and formalized in [Framester](https://github.com/framester/Framester).
ISAAC is supplied with a practical application, ImageSchemaNet which extends the Framester schema, operationalising image schemas in knowledge graphs extracted from text.




### LIst of ontology modules


[J87](http://www.ontologydesignpatterns.org/ont/is/j87.owl) ``http://www.ontologydesignpatterns.org/ont/is/j87.owl``

[MPC](http://www.ontologydesignpatterns.org/ont/is/mpc.owl) ``http://www.ontologydesignpatterns.org/ont/is/mpc.owl``

[HED](http://www.ontologydesignpatterns.org/ont/is/hed.owl) ``http://www.ontologydesignpatterns.org/ont/is/hed.owl``

[ISCAT](http://www.ontologydesignpatterns.org/ont/is/iscat.owl) ``http://www.ontologydesignpatterns.org/ont/is/iscat.owl``

[ISFrame](http://www.ontologydesignpatterns.org/ont/is/isframe.owl) ``http://www.ontologydesignpatterns.org/ont/is/isframe.owl``

[ISAAC](http://www.ontologydesignpatterns.org/ont/is/isaac.owl) ``http://www.ontologydesignpatterns.org/ont/is/isaac.owl``




### ISAAC ontology network in detail

ISAAC modular ontology includes three main theoretical modules:

**J87**

The ontological transposition of the first five chapters of Mark Johnson's "The Body in the Mind".
This theory was chosen because it is the beginning of the last 40 years of studies about embodied cognition, moving first steps in 1987 and still very alive and in need of further work.



**MPC**

The ontological version of [1](https://d1wqtxts1xzle7.cloudfront.net/39255761/54d803e90cf2970e4e764653.pdf?1445107592=&response-content-disposition=inline%3B+filename%3DOn_defining_image_schemas.pdf&Expires=1620342019&Signature=LcS38kkqdWTN3F6HumKPZ~xa4rIc8Q5MV2hevqclSLpmWsryhKI3496FcZwYljKbGeSNlvmfv-OBIOzCY37FGH4oedAVdHTNDzvNoVfdIQ7Zzru3daKdTWrypGIsKuGOHgwF46J7-Mr9SDoHtG7H9MeNA1TqHFNwhdt1xVQ62OuAuJk27kXSr1y~RHqVqTC7l~GbFVwQ9us8zzcWfUiLkFTX89rz3b0sGYdVpyze6PVEaYdYFY8DhQUgBFi5ppPbT9VkbwF5Akn7Y7WQ2Y18Vyms6n3LPSqNdnL-mEcOquBDxueaslGOZ~xruftZzTgYYxQPVxFHARRdDPbe7A0NDg__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA). This module was chosen for the importance of introducing spatial primitives, namely the first spatial building blocks, and introducing some light formalization in the compositionality of image schemas.



**HED**

The ontological version of the image schema theory elaborated by Hedblom et al. in [1](https://link.springer.com/article/10.1007/s13218-019-00605-1), [2](https://dl.acm.org/doi/abs/10.1145/3167132.3167233?casa_token=jA3_AHLyUroAAAAA:r1dve2UFBe2nfhN0nHn8irpKYRhH-MQdqbCpzvZvAJyNO8UzPJ6K3ZdBwOrN3T7ZTlOX4yPZQxU), [3](https://www.inf.unibz.it/~okutz/resources/Choosing-the-Right-Path_-Image-Schema-Theory-as-a-Foundation-for-Concept-Invention-(JAGI).pdf) and [4](http://aiia2017.di.uniba.it/wp-content/uploads/Hedblom.pdf).
This module was chosen for its importance in formalizing image schemas structure, image schemas combinations and image schemas complexity depending on the reuse of spatial primitives.



ISAAC imports the above mentioned modules and introduces some axioms and properties to perform cross-modular inferences.
Finally, some additional modules are being developed and integrated in the network.


**ISCAT**

The module obtained from the reorganization of [this resource](http://zope.psyergo.uni-wuerzburg.de/iscat) in a well documented CSV file available [here](https://github.com/dgromann/ImageSchemaRepository).


**ISFrame**

The mappings from ISCAT repository to FrameNet and MetaNet source and target domain frames, declaring also the spatial primitive / image schema gestaltically structuring the metaphor.





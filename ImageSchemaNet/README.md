
# Image Schema Net

Commonsense knowledge is a broad and challenging area of research which investigates our understanding of the world as well as human assumptions about reality.
Deriving directly from the subjective perception of the external world makes it intrinsically intertwined with embodied cognition. 
Commonsense reasoning in particular is linked to human sense-making, pattern recognition and knowledge framing abilities. 

ImageSchemaNet is a new resource that formalizes the cognitive theory of image schemas. 


Image schemas are described as dynamic conceptual building blocks originating from our sensorimotor interactions with the physical world, and enable our sense-making cognitive activity to assign coherence and structure to entities, events and situations we experience everyday.


ImageSchemaNet is an ontology that aligns pre-existing resources, such as FrameNet, VerbNet, WordNet and MetaNet from the Framester hub, to image schema theory, aiming at an empirical application of image schemas combined with sematic parsers on the task of annotating natural language sentences with image schemas.



### Explore the Resource! 

Query to ask if some entity is a lexical activator of some spatial primitive which is necessary to the image schemaCONTAINMENT.

ASK
?entity isnet:lexicalSenseActivation ?sp .
?sp ^isnet:necessarySP isnet:CONTAINMENT .




Query to retrieve all the entities, image schemas and spatial primitives for which some entity is a lexical activator of some SP which is a necessary SP to some IS.

SELECT DISTINCT ?entity ?is ?sp
WHERE {
?entity isnet:lexicalSenseActivation ?sp .
?sp ^isnet:necessarySP ?is .
FILTER(regex(?entity, "insert_variable", "i")) 
}




Query to simulate the image-schema-profile extraction starting from a single non disambiguated lexical unit.
The query can be executed by replacing each "insert_variable" with the same lexical unit.

CONSTRUCT { [] isnet:ISProfile ?isLex , ?coresp , ?perisp , ?etsp , ?semis, ?rolesp . }
WHERE {
{ ?x1 isnet:lexicalSenseActivation ?isLex .
FILTER(regex(?x1, "insert_variable", "i")) }
UNION
{ ?x2 isnet:coreSPActivation ?coresp .
FILTER(regex(?x2, "insert_variable", "i")) }
UNION
{ ?x3 isnet:peripheralSPActivation ?perisp .
FILTER(regex(?x3, "insert_variable", "i")) }
UNION
{ ?x4 isnet:extraThematicSPActivation ?etsp .
FILTER(regex(?x4, "insert_variable", "i")) }
UNION
{ ?x5 isnet:semTypeActivation ?semis .
FILTER(regex(?x5, "insert_variable", "i")) }
UNION
{ ?x6 isnet:semanticRoleActivation ?rolesp .
FILTER(regex(?x6, "insert_variable", "i")) }
}

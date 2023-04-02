# Formalization and Semantic enrichment of urban spaces for accessibility analysis 
Champions: TODO

## Challenge description:
The Semantic enrichment of large and complex geometric models such as city Digital Twins is crucial for the monitoring, understanding, simulation and prediction of phenomena that happen in the urban space. In particular, we will focus on accessibility, a problem of huge importance in a peculiar city like Matera. After being European capital of Culture in 2019 Matera has seen an enormous increase in touristic visits; besides, the age of tourists is gradually increasing and the accessibility of ancient sites and historical buildings might be problematic to some profiles of visitors, not to mention issues for impaired people. 

The semantics added to urban elements (platforms, streets, touristic attractions) can help understanding if a touristic route is appropriate to a specific visitor, according to his/her age, physical state, class of impairment, phobia or other factors. As examples, you may think of:
- The narrow, steep, uneven and slippery alleys in the Sassi district;
- The Palombaro Lungo, one of the top attractions, is underground, and is accessible through metallic steps high and narrow; illumination is also very low;
- The Tibetan bridge over the Gravina to access several rupestrian churches.

The geometry can provide numerical attributes that can possibly be automatically computed and explicitly annotated for efficient consultation. The challenge is the design of what to annotate and how to annotate in terms of classes and quantitative or qualitative attributes. You will need to model the visitor profile as well. The environmental conditions may also play a role (e.g., paths more slippery when wet) as well as other factors (e.g., number of people already occupying a public space for safety reasons).

Identify the urban elements that play a role in the assessment of accessibility (e.g., road, platform, stairs) and the attributes (quantitative or qualitative) relevant to describe each element (e.g., road->slope / roughness / …). Model the user according to his/her capacity / preferences /disabilities identifying the qualitative and quantitative attributes to be matched against the urban elements. The capacity may be intrinsic (e.g., difficulty to walk due to being overweight) or extrinsic (e.g., the person is carrying a trolley). You may decide the granularity of the description, maybe focussing on selected user types. 

## Challenger Research Questions:
- What are the most relevant urban elements for accessibility and what are the crucial attributes to be modelled? What attributes can and should be computed automatically from the 3D geometric model (e.g., because the attribute is crucial and must be computed precisely in many positions). Which semantics does the 3D model ideally need to be enriched with?
- Can you build an application interface which graphically aids the user to find a suitable route in the city of Matera, using the Matera Digital Twin, semantic attributes and user data?
- Optional: Model other boundary conditions (e.g., environmental conditions, thermal comfort) that may impact the level of accessibility / comfort of a path for a user.
- Optional: Information such as location and medical data is very sensitive. What measures can you take to guarantee the privacy of the user?

## Datasets available:
- 3D models of a few outdoor or indoor areas in Matera, represented as triangle meshes. 
- Generate your own user profiles (e.g. using the Solid ecosystem)

## Supplementary Resources
- https://publications.ergonomics.org.uk/uploads/The-challenge-of-cultural-heritage-visitation-A-problem-demanding-new-approaches.pdf

- A framework for the manual annotation of geometric regions (sets of adjacent triangles) developed by Andreas Scalas (CNR-IMATI) will be available to annotate urban elements according to the formalization produced. The software has a graphical user interface and allows to select regions and specify the class of the instance and the attributes. Geometric tools to compute the dimensions of the entity are given, e.g., a ruler to measure Euclidean distance) and can be used to define quantitative attributes.

- Solid Community Server (https://github.com/CommunitySolidServer/CommunitySolidServer)

## Tools
- Any IDE (e.g. VS Code)
- RDF-oriented environment (triple store, LDP, …)

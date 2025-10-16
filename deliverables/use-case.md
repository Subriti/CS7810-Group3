# Use-Case: CS Research Knowledge Graph


## Narrative  


Research in the field of Computer Science is one of the fastest-growing fields of science and technology, producing thousands of papers, patents, and grants each year. However, the information about this research is distributed across diverse platforms such as DBLP, NSF award databases, and USPTO patent repositories. This fragmentation creates challenges for researchers, funding agencies, students and policymakers who need to understand evolving trends, identify leading institutions, and explore collaboration and funding patterns. 


This Computer Science Research Knowledge Graph aims to integrate these three datasets into a unified semantic structure that represents the cycle of research — from funding → publications → innovation. By linking these sources, the graph will enable advanced analysis of how ideas spread, merge, and evolve across time and disciplines.

This project not only integrates data to model the dynamics of scientific progress but also leans towards:

Discovering the connections between papers – measuring conceptual similarity between research works.

Velocity of research – tracking how quickly research areas evolve, how topics emerge, and how innovations follow funding or publication.

Topic hierarchy – building a structured ontology of computer science domains (e.g., AI → Machine Learning → Deep Learning → Large Language Models), allowing researchers to navigate and reason about field evolution.


The **primary stakeholders** for this use-case are researchers, funding agencies, policymakers, industry leaders, and educators.  


- **Researchers** seek to identify emerging subfields, find potential collaborators, and track influential publications.  
- **Funding agencies** NSF and DARPA want to evaluate the impact of their grants, compare funding across CS subfields (e.g., NLP vs. Computer Vision), and optimize future investments.  
- **Policymakers and industry leaders** need to monitor the trajectory of CS technologies to inform regulations, national strategies, and innovation investments.  
- **Educators and students** can use the graph to explore the landscape of subfields in CS, visualize topic hierarchies and understand how concepts connect over time..  



A **Traditional relational (tabular) database** cannot easily represent or traverse the complex, many-to-many relationships between grants, papers, patents, authors, and institutions. A Knowledge Graph (KG), using semantic web captures these relationships explicitly and supports reasoning over them. This enables rich, cross-domain queries such as:

“Which NSF-funded research areas led to the most patents within five years?”
“What sequence of papers represents the evolution of deep learning?”
“How close are NLP and Computer Vision research in conceptual space?”

By modeling these semantic relationships, this KG can serve as a dynamic map of computer science research, showing the flow of ideas, collaborations, and innovations over time.

---


## Competency Questions 

1. Which NSF-funded projects resulted in the highest research and innovation velocity?
Bridges Datasets: NSF, DBLP, USPTO

2. How does research vary across different CS subfields?
Bridges Datasets: DBLP, NSF

3. What is the conceptual distance between two research papers or subfields?
Bridges Datasets: DBLP

4. Which institutions demonstrate the strongest link between funded research and patented outcomes?
Bridges Datasets: NSF, DBLP, USPTO

5. How much NSF funding has gone to NLP compared to Computer Vision research?  
*Bridges Datasets:* NSF Awards, DBLP  

6. Which AI patents cite academic research papers, and which institutions developed them?
*Bridges Datasets:* USPTO, DBLP

7. Which authors frequently publish in both academic venues (conferences/journals) and file patents?  
*Bridges Datasets:* DBLP, USPTO

8. Which institutions have received the most NSF grants related to AI research?  
*Bridges Datasets:* NSF Awards, DBLP

9. What hierarchical relationships exist among CS topics, and how do they evolve?
Bridges Datasets: DBLP

10. Which NSF-funded areas have produced patents most rapidly (shortest time lag)?
Bridges Datasets: NSF, DBLP, USPTO


---


## Potential Datasets  


1. **DBLP** – Computer science publication metadata (authors, venues, years).  
   - Source: https://dblp.org/xml/  
   - Accessed: September 30, 2025  


3. **US NSF Award Search Database** – Funding data for AI-related research projects.  
   - Source: https://www.nsf.gov/awardsearch/simpleSearchResult?queryText=artificial+intelligence
   - Accessed: September 30, 2025  


4. **USPTO Patent Database** – AI-related patents with inventors and institutions.  
   - Source: https://data.uspto.gov/patent-file-wrapper/bulkdata/entire
   - Accessed: September 30, 2025  



---


## Existing Resources  


- **OpenAlex** – An open catalog of scholarly papers, authors, and institutions. (https://openalex.org)  
- **Microsoft Academic Graph (retired)** – Historical dataset of publications and citations.  
- **OWL / RDF Standards** – For ontology development and semantic integration.  
- **Schema.org & Dublin Core** – Metadata standards for scholarly communication.  
- **AI-KG (Knowledge Graph of AI Publications)** – A previous project focusing on AI research papers.  


---


## References  


[1] T. Berners-Lee, J. Hendler, and O. Lassila, “The Semantic Web,” *Scientific American*, vol. 284, no. 5, pp. 34–43, May 2001. doi: 10.1038/scientificamerican0501-34.  


[2] C. Chen et al., “AI-KG: An Automatically Generated Knowledge Graph of Artificial Intelligence,” *Proceedings of CIKM 2020*, pp. 2973–2980.  


[3] OpenAlex. “OpenAlex: The open catalog of the global research system.” https://openalex.org (accessed Sep. 30, 2025).  


[4] National Science Foundation, “Award Search Database,” https://www.nsf.gov/awardsearch/ (accessed Sep. 30, 2025).  


[5] U.S. Patent and Trademark Office, “PatentsView Data,” https://www.uspto.gov/ (accessed Sep. 30, 2025).  


[6] arXiv.org, “arXiv API.” https://arxiv.org/help/api (accessed Sep. 30, 2025).  


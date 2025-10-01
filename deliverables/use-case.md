# Use-Case: AI Research Knowledge Graph

## Narrative  

Artificial Intelligence (AI) research is one of the fastest-growing fields of science and technology, producing thousands of papers, patents, and grants each year. However, the information about this research is distributed across diverse platforms such as DBLP, arXiv, NSF award databases, and USPTO patent repositories. This fragmentation creates challenges for researchers, funding agencies, and policymakers who need to understand evolving trends, identify leading institutions, and explore collaboration and funding patterns.  

The **primary stakeholders** for this use-case are researchers, funding agencies, policymakers, industry leaders, and educators.  

- **Researchers** seek to identify emerging subfields, find potential collaborators, and track influential publications.  
- **Funding agencies** like NSF and DARPA want to evaluate the impact of their grants, compare funding across AI subfields (e.g., NLP vs. Computer Vision), and optimize future investments.  
- **Policymakers and industry leaders** need to monitor the trajectory of AI technologies to inform regulations, national strategies, and innovation investments.  
- **Educators and students** can use the graph to explore the landscape of AI subfields, locate relevant datasets, and study collaboration patterns.  

Building a **Knowledge Graph (KG)** for AI research is important because it enables the integration of heterogeneous data sources into a single semantic structure. This makes it possible to connect research papers, authors, institutions, patents, grants, and topics, allowing complex queries such as:  
- *“Which universities publish the most on Large Language Models?”*  
- *“What are the fastest-growing AI subfields in the last 5 years?”*  
- *“How much NSF funding has gone into NLP versus Computer Vision research?”*  

These insights would not be easily retrievable using isolated datasets.  

A **relational (tabular) database** is insufficient for this use-case because it enforces rigid schemas and lacks native support for relationships across multiple datasets. For example, linking an NSF grant to the papers it funded, the institutions that received it, and patents citing those papers requires traversing many-to-many relationships. A **Knowledge Graph**, however, naturally encodes these entities and relationships, supports reasoning via ontologies, and enables semantic queries with SPARQL. This flexibility allows researchers and decision-makers to extract actionable insights that would be extremely difficult or impossible in relational systems.  

Thus, the AI Research Knowledge Graph is both intellectually challenging and societally impactful. It will integrate diverse datasets, model meaningful relationships, and provide a foundation for advanced analytics and visualization of AI research trends.  

---

## Competency Questions  

1. What are the fastest-growing AI subfields in the last 5 years?  
*Bridges Datasets:* DBLP, arXiv  

2. Which universities publish the most on Large Language Models (LLMs)?  
*Bridges Datasets:* DBLP, arXiv, Institution metadata  

3. Which researchers collaborate most frequently across different AI subfields?  
*Bridges Datasets:* DBLP, arXiv 

4. How much NSF funding has gone to NLP compared to Computer Vision research?  
*Bridges Datasets:* NSF Awards, DBLP, arXiv  

5. Which AI patents cite academic research papers, and which institutions developed them? 
*Bridges Datasets:* USPTO.org, DBLP, arXiv, Institution metadata  

6. Which authors frequently publish in both academic venues (conferences/journals) and file patents?  
*Bridges Datasets:* DBLP, arXiv, USPTO/Lens.org 

7. What are the top conferences and journals publishing AI/ML papers by volume?  
*Bridges Datasets:* DBLP, arXiv  

8. Which institutions have received the most NSF grants related to AI research?  
*Bridges Datasets:* NSF Awards, Institution metadata 

9. How has the volume of AI research papers evolved over time, broken down by subfield (e.g., NLP, Robotics, Computer Vision)?  
*Bridges Datasets:* DBLP, arXiv 

10. What collaborations exist between academia and industry labs in AI research outputs? 
*Bridges Datasets:* DBLP, arXiv, Institution metadata 

11. Which research topics are most strongly connected to recent breakthroughs in generative AI?  
*Bridges Datasets:* arXiv, DBLP  

12. Which institutions or labs show the strongest cross-disciplinary collaborations in AI subfields?  
*Bridges Datasets:* DBLP, arXiv, Institution metadata 

---

## Potential Datasets  

1. **DBLP** – Computer science publication metadata (authors, venues, years).  
   - Source: https://dblp.org/xml/  
   - Accessed: September 30, 2025  

2. **arXiv API** – AI/ML research papers, abstracts, and categories.  
   - Source: https://arxiv.org/help/api/  
   - Accessed: September 30, 2025  

3. **NSF Award Search Database** – Funding data for AI-related research projects.  
   - Source: https://www.nsf.gov/awardsearch/  
   - Accessed: September 30, 2025  

4. **USPTO Patent Database** – AI-related patents with inventors and institutions.  
   - Source: https://data.uspto.gov/patent-file-wrapper/bulkdata/entire
   - Accessed: September 30, 2025  

5. **Lens.org** – Global patent and scholarly data linked to institutions and inventors.  
   - Source: https://www.lens.org/  
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
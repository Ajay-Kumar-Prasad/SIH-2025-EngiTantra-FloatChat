# 🌊 SIH-2025-FloatChat

**AI-Powered Conversational System for ARGO Float Data**

This repository is a Smart India Hackathon 2025 project that aims to democratize access to **oceanographic data** by enabling users to query, explore, and visualize **ARGO float datasets** using **natural language**.  

---

## 📌 Background  

Oceanographic data is vast, complex, and heterogeneous – ranging from satellite observations to in-situ measurements like CTD casts, Argo floats, and BGC sensors.  

The **Argo program**, which deploys autonomous profiling floats across the world’s oceans, generates an extensive dataset in **NetCDF format**, containing temperature, salinity, and other essential variables.  

However, accessing and making sense of this data requires technical expertise and familiarity with specialized tools.  

With the rise of **AI & Large Language Models (LLMs)** combined with **structured databases** and **interactive dashboards**, it is now possible to build intuitive, conversational systems that **bridge the gap between raw ocean data and decision-makers**.  

---

## 🎯 Problem Statement  

Develop an **AI-powered conversational system for ARGO float data** that enables users to:  
- Query oceanographic datasets in **natural language**  
- Retrieve, process, and visualize **ARGO float profiles**  
- Explore geospatial and temporal insights interactively  

---

## 🛠️ System Description  

The proposed system will:  

- **Data Processing**  
  - Ingest ARGO **NetCDF files**  
  - Convert data into structured formats (SQL, Parquet)  

- **Storage & Retrieval**  
  - Store structured data in a **relational database** (PostgreSQL)  
  - Store metadata & summaries in a **vector database** (FAISS / Chroma)  

- **AI-Powered Querying**  
  - Use **Retrieval-Augmented Generation (RAG)** pipelines with multimodal LLMs (GPT, QWEN, LLaMA, Mistral)  
  - Interpret user queries and map them into **SQL/database queries**  
  - Implement **Model Context Protocol (MCP)** for structured AI-agent interactions  

- **Visualization & Interaction**  
  - Interactive dashboards via **Streamlit** or **Dash**  
  - Support visualizations like:  
    - Mapped ARGO float trajectories  
    - Depth-time plots  
    - Profile comparisons  
  - Export results as **ASCII / NetCDF**  

- **Chat Interface**  
  - Conversational UI for non-technical users  
  - Example queries:  
    - *"Show me salinity profiles near the equator in March 2023"*  
    - *"Compare BGC parameters in the Arabian Sea for the last 6 months"*  
    - *"What are the nearest ARGO floats to this location?"*  

---

## ✅ Expected Solution  

- End-to-end pipeline to **process ARGO NetCDF data** and store in **PostgreSQL + FAISS/Chroma**  
- Backend powered by **LLMs** for **natural language to SQL** translation  
- Interactive frontend dashboard for **geospatial & temporal visualizations**  
- **Chatbot interface** for guided data exploration  
- Proof-of-Concept with **Indian Ocean ARGO data**  
- Extensible to **BGC floats, gliders, buoys, satellite datasets**  

---

## 📂 Repository Structure  
```
SIH-2025-FloatChat/
├── code/ # Source code
│ ├── backend/ # APIs, database connectors, RAG pipeline
│ ├── frontend/ # Streamlit/Dash dashboard & chatbot UI
│ └── data/ # Sample ARGO NetCDF files, SQL/Parquet outputs
│
├── docs/ # Documentation
│ ├── approach.md 
│ └── architecture.png
│
├── demo/ # Demo videos, screenshots, sample outputs
│
├── ppt/ # SIH pitch deck
│
├── .gitignore
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

---

## 📖 Acronyms  

- **NetCDF**: Network Common Data Format  
- **CTD**: Conductivity Temperature and Depth  
- **BGC**: Bio-Geo-Chemical Floats  

---

## 🚀 Tech Stack  

- **Databases:** PostgreSQL, FAISS/Chroma  
- **AI/ML:** LLMs (GPT, QWEN, LLaMA, Mistral), RAG Pipelines, MCP  
- **Visualization:** Plotly, Leaflet, Cesium, Streamlit/Dash  
- **Data Format:** NetCDF, Parquet, ASCII  


---

## 👥 Team Members  

<!-- Add contributors here -->
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Ajay-Kumar-Prasad">
        <img src="https://github.com/Ajay-Kumar-Prasad.png" width="100px;" alt="SOHAM-3T"/>
        <br />
        <sub><b>Ajay Kumar Prasad</b></sub>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://github.com/SOHAM-3T">
        <img src="https://github.com/SOHAM-3T.png" width="100px;" alt="SOHAM-3T"/>
        <br />
        <sub><b>Soham Tripathy</b></sub>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://github.com/SaiPrithvi1278">
        <img src="https://github.com/SaiPrithvi1278.png" width="100px;" alt="SOHAM-3T"/>
        <br />
        <sub><b>Sai Prithvi</b></sub>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://github.com/NetsNuts-24">
        <img src="https://github.com/NetsNuts-24.png" width="100px;" alt="Neti"/>
        <br />
        <sub><b>Neti Dubey</b></sub>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://github.com/jeevan1276">
        <img src="https://github.com/jeevan1276.png" width="100px;" alt="Jeevan"/>
        <br />
        <sub><b>Manepalli Jeevan</b></sub>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://github.com/jeevan1276">
        <img src="https://github.com/jeevan1276.png" width="100px;" alt="Jeevan"/>
        <br />
        <sub><b>Manepalli Jeevan</b></sub>
      </a>
      <br/>
    </td>
    <td align="center">
      <a href="https://github.com/Surya070805">
        <img src="https://github.com/Surya070805.png" width="100px;" alt="Surya"/>
        <br />
        <sub><b>Surya Mitra</b></sub>
      </a>
      <br/>
    </td>
  </tr>
</table>
---

## 🤝 Contributing  
1. Fork this repo  
2. Create your branch: `git checkout -b feature-name`  
3. Commit changes: `git commit -m "Added new feature"`  
4. Push branch: `git push origin feature-name`  
5. Submit Pull Request 

## Note:
For now focus on creating Documentation...

---

## 🤝 Contribution  

We welcome contributions! Please check out the [CONTRIBUTING.md](CONTRIBUTING.md) file for details on how to get started.  

---

## 📜 License  

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.  

---

### 🌊 Empowering Ocean Research with AI  
This project bridges the gap between **ocean data complexity** and **real-world accessibility** for scientists, policymakers, and non-technical users.  


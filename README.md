# Mapa de Autoridades de Ciberseguridad en México

En México existe una **proliferación de instrumentos normativos y administrativos** que crean autoridades y les otorgan facultades en el **ámbito de la ciberseguridad y la seguridad de la información**. Esa dispersión provoca **solapamientos de atribuciones**, vacíos de coordinación y decisiones públicas desalineadas.

Este repositorio nace como un **proyecto colaborativo y practitioner** para **identificar, ordenar y describir** a las autoridades que actúan en este dominio, mostrando en un mismo lugar:
- **Autoridad / Órgano**
- **Nivel de gobierno**
- **Sector / ámbito**
- **Tipo de rol en ciberseguridad**
- **Funciones relacionadas con ciberseguridad (síntesis)**
- **Fundamento legal (norma, art., fracción)**
- **Notas / limitaciones**

> **Tablas completas por rubro:**  
> ➜ [`organizacion_autoridades_por_rubros.md`](./organizacion_autoridades_por_rubros.md)

---

## ¿Qué problema resuelve?
El **sistema jurídico-administrativo** en ciberseguridad está **fragmentado** y carece de un mapeo público consolidado. Este proyecto facilita una **vista clara y verificable** para evitar duplicidades, entender **quién hace qué** y sostener decisiones informadas.

---

## Alcance: rubros y roles

**Rubros principales (ejemplos):**
- Gobernanza y rectoría federal
- Seguridad nacional e inteligencia
- Seguridad pública y prevención del delito
- Sector financiero
- Sector energético: hidrocarburos y gas natural; energía eléctrica; nuclear
- Poder Judicial y justicia
- Procuración de justicia
- Protección de datos personales
- Telecomunicaciones
- Transporte y aviación
- Hacienda y administración tributaria
- Educación
- Salud
- Vivienda y seguridad social
- Estadística y geografía
- Anticorrupción y transparencia
- Género y protección de víctimas
- Recursos hídricos y medio ambiente
- Archivos y gestión documental
- Población e identidad
- Electoral
- Política exterior
- Consumo y comercio electrónico
- Propiedad intelectual
- Otras direcciones generales TIC sectoriales

**Tipos de rol (estandarizados):**  
**Normativo/Regulador · Supervisor · Operativo/CSIRT · Coordinación · Inteligencia · Diplomacia · Operación institucional**

---

## ¿Para quién es útil?
- **Legisladores y congresos** (federal y locales)
- **Policymakers** y diseñadores de política pública
- **Reguladores sectoriales** y **autoridades coordinadoras**
- **Empresas** (incl. operadores de infraestructura crítica) y **cámaras**
- **CSIRTs**, **equipos de respuesta**, **equipos de cumplimiento**
- **Academia**, **investigadores**, **think tanks**
- **Sociedad civil** y **periodismo especializado**

 ---  

## Cómo leer el repositorio
- La **tabla por rubros** concentra la información estructurada, con su **fundamento legal** y **notas** de alcance o limitaciones.  
  ➜ [`organizacion_autoridades_por_rubros.md`](./organizacion_autoridades_por_rubros.md)

- El **diagrama** ofrece una vista de alto nivel del ecosistema y relaciones.

<details>
<summary><strong>Ver diagrama (Mermaid)</strong></summary>

```mermaid
graph LR
    Root[ECOSISTEMA CIBERSEGURIDAD MÉXICO 87+ autoridades]
    
    Root --> Cat1[RECTORÍA Y SEGURIDAD]
    Root --> Cat2[SECTORES FINANCIERO Y ENERGÉTICO]
    Root --> Cat3[JUSTICIA Y PROTECCIÓN]
    Root --> Cat4[OTROS SECTORES]
    Root --> Cat5[ADMINISTRACIÓN INSTITUCIONAL]
    
    Cat1 --> SG1
    Cat1 --> SG2
    Cat1 --> SG3
    Cat1 --> SG4
    
    subgraph SG1["RECTORÍA"]
        A1["DG Ciberseguridad ATDT"]
        A2["ATDT Autoridad Nacional"]
    end
    
    subgraph SG2["SEGURIDAD NACIONAL"]
        B1[CNI]
        B2[SESNSP]
        B3["SEDENA COC"]
        B4["SEMAR EMCOGCIBER"]
    end
    
    subgraph SG3["SEGURIDAD PÚBLICA"]
        C1["SSPC Unidad Inteligencia"]
        C2["SSPC DG Investigación"]
        C3["SSPC Infraestructura"]
        C4["SSPC DG Plataforma"]
        C5["GN DG Científica"]
        C6["Policías Cibernéticas 32"]
        C7["Consejo Nacional"]
        C8["Comité Ciberseguridad"]
    end
    
    subgraph SG4["PROCURACIÓN"]
        D1["FGR Infraestructura"]
        D2["FGR Consejo"]
        D3["FGR Gobernanza"]
        D4["FGR CENAPI"]
    end
    
    Cat2 --> SG5
    Cat2 --> SG6
    Cat2 --> SG7
    Cat2 --> SG8
    
    subgraph SG5["FINANCIERO"]
        E1["Banxico Dir Ciber"]
        E2["Banxico Comité"]
        E3["Banxico SPEI"]
        E4[CNBV]
        E5["CNBV CUB"]
        E6["CNBV IFPE"]
        E7[CNSF]
        E8[CONSAR]
        E9[IPAB]
        E10["Comité ITF"]
        E11[CONDUSEF]
        E12[UIF]
    end
    
    subgraph SG6["ENERGÍA HIDRO"]
        F1["CENAGAS Jefatura"]
        F2["CENAGAS Dir Infra"]
        F3["Pemex Coord"]
        F4["Pemex Gerencia"]
        F5[IMP]
        F6[ASEA]
        F7["CNH CNIH"]
    end
    
    subgraph SG7["ENERGÍA ELÉCTRICA"]
        G1[CENACE]
        G2["CFE Distribución"]
        G3["CFE Generación"]
        G4["CFE TEIT"]
        G5["CFE Suministrador"]
        G6["CFE Transmisión"]
        G7[CRE]
    end
    
    subgraph SG8["NUCLEAR"]
        H1[CNSNS]
    end
    
    Cat3 --> SG9
    Cat3 --> SG10
    
    subgraph SG9["PODER JUDICIAL"]
        I1["SCJN Comisión"]
        I2["SCJN DG TI"]
        I3["CJF Facilitadoras"]
        I4["CJF SNIJ"]
        I5["Poderes Judiciales"]
        I6[TFJA]
        I7[TEPJF]
    end
    
    subgraph SG10["DATOS Y ELECTORAL"]
        J1["SABG Público"]
        J2["Autoridades Garantes"]
        J3["SABG Privado"]
        J4["INE UTSI"]
    end
    
    Cat4 --> SG11
    Cat4 --> SG12
    
    subgraph SG11["TELECOM Y TRANSPORTE"]
        K1[CRT]
        K2[AFAC]
        K3[ASIPONA]
    end
    
    subgraph SG12["OTROS REGULADOS"]
        L1["Salud NOM-024"]
        L2[PROFECO]
        L3["SE PSC"]
        L4[IMPI]
        L5[INDAUTOR]
    end
    
    Cat5 --> SG13
    Cat5 --> SG14
    Cat5 --> SG15
    
    subgraph SG13["HACIENDA Y EDUCACIÓN"]
        M1["SHCP Coord SI"]
        M2["SAT AGCTI"]
        M3[ANAM]
        M4[CONALEP]
        M5[IPN]
        M6[SEP]
    end
    
    subgraph SG14["ESTADÍSTICA Y OTROS"]
        N1[INEGI]
        N2[INFONAVIT]
        N3[SNA]
        N4[ASF]
        N5["Sec Mujeres"]
    end
    
    subgraph SG15["GOBIERNO INSTITUCIONAL"]
        O1[CONAGUA]
        O2[SEMARNAT]
        O3[AGN]
        O4["SEGOB RENAPO"]
        O5["SEGOB TIC"]
        O6["SRE ONU"]
        O7["SRE Globales"]
        O8["SRE TI"]
        O9[SICT]
        O10["Otras DG TIC"]
    end
    
    style Root fill:#2c3e50,color:#fff,stroke:#34495e,stroke-width:4px
    style Cat1 fill:#e74c3c,color:#fff,stroke:#c0392b,stroke-width:3px
    style Cat2 fill:#16a085,color:#fff,stroke:#138d75,stroke-width:3px
    style Cat3 fill:#8e44ad,color:#fff,stroke:#7d3c98,stroke-width:3px
    style Cat4 fill:#f39c12,color:#fff,stroke:#d68910,stroke-width:3px
    style Cat5 fill:#95a5a6,color:#fff,stroke:#7f8c8d,stroke-width:3px

```
</details>

---
## 🤝 Sugerencias y mejoras

Este mapa está en evolución. Si encuentras una autoridad faltante, un fundamento por afinar o una mejor forma de clasificar, será un gusto leerte.

**Contacto:** https://mx.linkedin.com/in/jersain

**Formato sugerido (copia y pega en tu mensaje):**
- Autoridad / Órgano:
- Nivel de gobierno:
- Sector / ámbito:
- Rol en ciberseguridad:
- Funciones (2-4 líneas):
- Fundamento legal (instrumento + art./fracc. + DOF + URL oficial):
- Notas / limitaciones:

---
[![Licencia: CC BY-NC-SA 4.0](https://img.shields.io/badge/Licencia-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
---

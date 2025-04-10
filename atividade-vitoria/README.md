# Pseudo-Cores Naturais (Vitória/ES)

## Objetivo
Criar uma composição de pseudo-cores naturais (PCN) para o município de Vitória/ES utilizando bandas do satélite Landsat 8, destacando:
- Áreas urbanas
- Cobertura vegetal
- Corpos d'água

---

## Metodologia
1. **Dados Utilizados:**
   - Imagens Landsat 8 (Bandas 3, 4, 5)
   - Shapefile de Vitória (IBGE, código 3205309)

2. **Processamento no QGIS:**
   - Recorte do raster pela área municipal (`Recortar raster por máscara`)
   - Composição RGB personalizada:
     - **Vermelho (R):** Banda 4 (Vermelho)
     - **Verde (G):** Banda sintética `0.65*banda 4 + 0.35*banda5`
     - **Azul (B):** Banda sintética `0.85*banda 3 - 0.15*banda 5`

3. **Sistema de Referência:**
   - **CRS:** SIRGAS 2000 / UTM zone 24S (EPSG:31984)
   - **Resolução espacial:** 30m
  
  ## Resultados


---

## Referências
- [IBGE - Malhas Municipais](https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-digitais.html)
- [USGS - Landsat 8](https://www.usgs.gov/landsat-missions/landsat-8)
- [Documentação do QGIS](https://qgis.org/pt_BR/docs/index.html)
- [Canal Mundo Geomática](https://www.youtube.com/@mundogeomatica/featured)

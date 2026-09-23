# Geoportal — Ilhas de Calor x Arborização (Jaguariúna)

Geoportal interativo para visualização cruzada entre ilhas de calor urbanas e cobertura de arborização no município de Jaguariúna/SP.

🔗 **Acesse ao vivo:** https://mirianniz-debug.github.io/IlhaCalorArborizacao/

## Sobre

Mapa web que permite consultar e comparar espacialmente áreas com maior intensidade de ilha de calor e a distribuição da arborização urbana, servindo de apoio a análises de conforto térmico e planejamento urbano/ambiental.

## Tecnologias

- Leaflet.js
- QGIS (exportado via QGIS2Web)
- HTML/CSS/JavaScript puro (sem build/dependências)

## Como visualizar localmente

Não há dependências ou build — basta abrir `index.html` diretamente no navegador, ou servir a pasta com um servidor estático simples:

```bash
python3 -m http.server 8000
```

Depois acesse `http://localhost:8000` no navegador.

## Incorporando o geoportal em outro site (iframe)

O `index.html` é responsivo, mas isso só funciona se o `<iframe>` que o incorpora também for responsivo. Use sempre largura em porcentagem, nunca um valor fixo em pixels:

```html
<iframe src="URL_DO_GEOPORTAL" style="width:100%; border:0;" height="600" loading="lazy"></iframe>
```

## Licença

Todos os direitos reservados. Ver [LICENSE](LICENSE).

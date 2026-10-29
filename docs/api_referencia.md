# 1. Crear y cambiar a una nueva rama
git checkout -b feature/api-reference

# 2. Crear el archivo docs/api_referencia.md con contenido
echo "# Referencia de la API" > docs/api_referencia.md
echo "" >> docs/api_referencia.md
echo "## Endpoints principales" >> docs/api_referencia.md
echo "" >> docs/api_referencia.md
echo "### GET /api/consumo" >> docs/api_referencia.md
echo "Devuelve el consumo energético del usuario." >> docs/api_referencia.md
echo "" >> docs/api_referencia.md
echo "### POST /api/consumo" >> docs/api_referencia.md
echo "Registra un nuevo consumo." >> docs/api_referencia.md
echo "" >> docs/api_referencia.md
echo "### DELETE /api/consum/{id}" >> docs/api_referencia.md
echo "Elimina un registro de consumo." >> docs/api_referencia.md

# 3. Añadir y hacer commit
git add docs/api_referencia.md
git commit -m "docs: añadir referencia de la API"

# 4. Subir la rama
git push origin feature/api-reference
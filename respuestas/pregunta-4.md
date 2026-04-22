MATCH (e:Empresa {nombre: 'TechCorp'})<-[:TRABAJA_EN]-(p:Persona)-[:VIVE_EN]->(c:Ciudad)
RETURN DISTINCT c.nombre AS Ciudad
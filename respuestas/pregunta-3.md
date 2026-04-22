MATCH (p:Persona)-[:PARTICIPA_EN]->(pr:Proyecto)
RETURN pr.nombre AS Proyecto, count(p) AS NumeroParticipantes
ORDER BY NumeroParticipantes DESC
LIMIT 2
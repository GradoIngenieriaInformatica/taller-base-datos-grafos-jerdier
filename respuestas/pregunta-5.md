MATCH (p:Persona)-[:TRABAJA_EN]->(e:Empresa)
MATCH (p)-[:VIVE_EN]->(c:Ciudad)
RETURN p.nombre AS Empleado, e.nombre AS Empresa, c.nombre AS Ciudad
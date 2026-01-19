# Diseño de Red – SecurityX

Este documento describe el diseño de red del laboratorio SecurityX, orientado a simular una infraestructura empresarial segura.

## Objetivo
Implementar una red segmentada y controlada mediante un firewall central, reduciendo la superficie de ataque y el movimiento lateral.

## Topología
La red está segmentada en varias zonas, cada una con una función específica:

- LAN Usuarios
- Servidores (VLAN20)
- DMZ
- Red de Gestión

Todas las redes pasan obligatoriamente por pfSense.

## Segmentación de Red

| Red | Subred | Función |
|----|-------|--------|
| LAN | 192.168.50.0/24 | Usuarios |
| VLAN20 | 192.168.2.0/24 | Servidores |
| DMZ | 192.168.3.0/24 | Servicios públicos |
| Gestión | 192.168.4.0/24 | Administración |

## Justificación de Seguridad
La segmentación permite:
- Limitar accesos entre redes
- Reducir impacto ante compromisos
- Controlar todo el tráfico desde el firewall

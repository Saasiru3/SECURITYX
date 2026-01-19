# Configuración de Seguridad – SecurityX

Este documento describe las medidas de seguridad implementadas en el laboratorio SecurityX.

## Firewall
pfSense actúa como firewall central y gateway de todas las redes.

## Reglas Principales
- Tráfico permitido solo cuando es necesario
- Acceso a red de gestión restringido
- Reglas separadas por interfaz
- Política de denegación por defecto

## NAT
Se implementa NAT controlado para permitir acceso a servicios públicos en DMZ.

## IDS – Suricata
Suricata se despliega como IDS para monitorizar tráfico sospechoso.

## Objetivo de Seguridad
- Detectar tráfico malicioso
- Registrar eventos
- Simular tareas de análisis SOC

---
author: JuanHV
creado: <% tp.file.creation_date() %>
modificado: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm:ss")%>
type: Patologías
tags: #Patologia
description:
tema: <%tp.file.title%>
---

# [[<%tp.file.title%>]]

<% await tp.file.move("/Patologías/" + tp.file.title) %>

## Definicion

## Epidemiologia

## Etiologia

## Fisiopatologia

## Cuadro Clinico

## Diagnostico

## Tratamiento


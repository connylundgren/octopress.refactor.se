---
author: connylundgren
date: '2007-09-03 18:54:03'
layout: post
slug: jsf-tags-reference
status: publish
title: JSF tags reference
wordpress_id: '109'
categories:
- JSF
comments: true
---

While working on some custom renderers last week I one again found myself
searching for the Component Type and Family for any given renderer, so here is
a compilation of render-types for future reference.

Say what you want about JSF, but the concept of renderers is a feature I
really like, and is one area where JSF actually shines (No this is not
intended as flame bait).

Tag Name Component Family Component Type Renderer Type

h:column

javax.faces.Column

javax.faces.Column

-

h:commandButton

javax.faces.Command

javax.faces.HtmlCommandButton

javax.faces.Button

h:commandLink

javax.faces.Command

javax.faces.HtmlCommandLink

javax.faces.Link

h:dataTable

javax.faces.Data

javax.faces.HtmlDataTable

javax.faces.Table

h:form

javax.faces.Form

javax.faces.HtmlForm

javax.faces.Form

h:graphicImage

javax.faces.Graphic

javax.faces.HtmlGraphicImage

javax.faces.Image

h:inputHidden

javax.faces.Input

javax.faces.HtmlInputHidden

javax.faces.Hidden

h:inputSecret

javax.faces.Input

javax.faces.HtmlInputSecret

javax.faces.Secret

h:inputText

javax.faces.Input

javax.faces.HtmlInputText

javax.faces.Text

h:inputTextarea

javax.faces.Input

javax.faces.HtmlInputTextarea

javax.faces.Textarea

h:message

javax.faces.Message

javax.faces.HtmlMessage

javax.faces.Message

h:messages

javax.faces.Messages

javax.faces.HtmlMessages

javax.faces.Messages

h:outputFormat

javax.faces.Output

javax.faces.HtmlOutputFormat

javax.faces.Format

h:outputLabel

javax.faces.Output

javax.faces.HtmlOutputLabel

javax.faces.Label

h:outputLink

javax.faces.Output

javax.faces.HtmlOutputLink

javax.faces.Link

h:outputText

javax.faces.Output

javax.faces.HtmlOutputText

javax.faces.Text

h:panelGrid

javax.faces.Panel

javax.faces.HtmlPanelGrid

javax.faces.Grid

h:panelGroup

javax.faces.Panel

javax.faces.HtmlPanelGroup

javax.faces.Group

h:selectBooleanCheckbox

javax.faces.SelectBoolean

javax.faces.HtmlSelectBooleanCheckbox

javax.faces.Checkbox

h:selectManyCheckbox

javax.faces.SelectMany

javax.faces.HtmlSelectManyCheckbox

javax.faces.Checkbox

h:selectManyListbox

javax.faces.SelectMany

javax.faces.HtmlSelectManyListbox

javax.faces.Listbox

h:selectManyMenu

javax.faces.SelectMany

javax.faces.HtmlSelectManyMenu

javax.faces.Menu

h:selectOneListbox

javax.faces.SelectOne

javax.faces.HtmlSelectOneListbox

javax.faces.Listbox

h:selectOneMenu

javax.faces.SelectOne

javax.faces.HtmlSelectOneMenu

javax.faces.Menu

h:selectOneRadio

javax.faces.SelectOne

javax.faces.HtmlSelectOneRadio

javax.faces.Radio


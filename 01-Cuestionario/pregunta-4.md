<?xml version="1.0" encoding="UTF-8"?>
<!-- This example adapted from the PET Handbook, copyright University of Cambridge ESOL Examinations -->
<assessmentItem xmlns="http://www.imsglobal.org/xsd/imsqti_v2p1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xsi:schemaLocation="http://www.imsglobal.org/xsd/imsqti_v2p1 http://www.imsglobal.org/xsd/qti/qtiv2p1/imsqti_v2p1.xsd" 
identifier="choice" 
title="Pregunta 4" 
adaptive="false" 
timeDependent="false"> 
<responseDeclaration identifier="RESPONSE_4" cardinality="single" baseType="identifier">
    <correctResponse>
        <value>ChoiceB</value>
    </correctResponse>
</responseDeclaration>
<outcomeDeclaration identifier="SCORE" cardinality="single" baseType="float">
    <defaultValue>
        <value>0</value>
    </defaultValue>
</outcomeDeclaration>
<itemBody>
    <p>¿El mejor amigo del hombre es el...?</p>
    <choiceInteraction responseIdentifier="RESPONSE_4" shuffle="false" maxChoices="1">
        <simpleChoice identifier="ChoiceA">Pes</simpleChoice>
        <simpleChoice identifier="ChoiceB">Prase</simpleChoice>
        <simpleChoice identifier="ChoiceC">Kočka</simpleChoice>
    </choiceInteraction>
</itemBody>
<responseProcessing
template="http://www.imsglobal.org/question/qti_v2p2/rptemplates/match_correct"/>
</assessmentItem>
<?xml version="1.0" encoding="UTF-8"?>
<!-- This example adapted from the PET Handbook, copyright University of Cambridge ESOL Examinations -->
<assessmentItem xmlns="http://www.imsglobal.org/xsd/imsqti_v2p1" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xsi:schemaLocation="http://www.imsglobal.org/xsd/imsqti_v2p1 http://www.imsglobal.org/xsd/qti/qtiv2p1/imsqti_v2p1.xsd" 
identifier="choice" 
title="Pregunta 1" 
adaptive="false" 
timeDependent="false">  
    <responseDeclaration identifier="RESPONSE_1" cardinality="single" baseType="identifier">
        <correctResponse>
            <value>ChoiceA</value>
        </correctResponse>
    </responseDeclaration>
        <outcomeDeclaration identifier="SCORE" cardinality="single" baseType="float">
        <defaultValue>
            <value>0</value>
        </defaultValue>
    </outcomeDeclaration>
        <itemBody>
        <p>¿Cómo se saluda de modo informal en checo?</p>
        <choiceInteraction responseIdentifier="RESPONSE_1" shuffle="false" maxChoices="1">
            <simpleChoice identifier="ChoiceA">Ahoj</simpleChoice>
            <simpleChoice identifier="ChoiceB">Nashledanou</simpleChoice>
            <simpleChoice identifier="ChoiceC">Sbohem</simpleChoice>
        </choiceInteraction>
    </itemBody>   
    <responseProcessing
        template="http://www.imsglobal.org/question/qti_v2p2/rptemplates/match_correct"/>
</assessmentItem>

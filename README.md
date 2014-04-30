LiveValidation
==============

Wiki macros implementation of the [LiveValidation javascript framework](http://livevalidation.com/documentation) to be used with validation specified in XWiki classes.

Macros
======

<table>
<tr><td><code>{{livevalidation /}}<td>Provides client-side live validation of a single XObject based on the validation expressions and messages defined in its XClass.
<tr><td><code>{{livevalidationCustom /}}<td>Validates a XObject property value using a custom remote XWiki document that should returns "true" when valid or "false" when not valid, based on the field value and the property reference.
<tr><td><code>{{livevalidationEmail /}}<td>Validates that XObject property value is a valid email address.
<tr><td><code>{{livevalidationFormat /}}<td>Validates that XObject property value against a regular expression.
<tr><td><code>{{livevalidationPresence /}}<td>Validates that XObject property value is present (ie. not null, undefined, or an empty string).
</table>

Usage
=====

``{{livevalidation form='inline' object='objectReference' /}}``

``{{livevalidationPresence form='formId' property='propertyReference' failureMessage='Non empty value required.' /}}``

``{{livevalidationFormat form='formId' property='propertyReference' pattern='[A-Z]+' failureMessage='Only uppercase characters allowed.' /}}``

``{{livevalidationEmail form='formId' property='propertyReference' failureMessage='Email format invalid.' /}}``

``{{livevalidationCustom form='formId' property='propertyReference' against='validationDocumentReference' failureMessage='Invalid value.'/}}``

For more, see the documentation of this module on [XWiki Extensions](http://extensions.xwiki.org/xwiki/bin/view/Extension/LiveValidation).

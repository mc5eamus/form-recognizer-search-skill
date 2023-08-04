# Azure Form Recognizer skill for Azure Cognitive Search

## Description
Azure Cognitive Search custom skill for entity extraction with Azure Form Recognizer

## Configuration 
### Environment Settings
Function Configuration / Application Settings or local.settings.json for local testing required:
* FORMS_RECOGNIZER_ENDPOINT
* FORMS_RECOGNIZER_KEY
* FORMS_RECOGNIZER_MODEL_ID

### Field Mapping
field_mappings.json defines key-value pairs with the key being the field name exposed by the Forms Recognizer model and the value as the property name within the "extracted" object returned by the function, make sure to reflect the changes in the outputFieldMappings of the indexer

### Skillset
Update the URI in the skillset to match the function AnalyzeForm endpoint URL

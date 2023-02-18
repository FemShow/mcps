# mcps

mcps-new-context.json is a JSON document that describes a QUBE configuration. QUBE is a tool that allows for the creation and management of datasets in CSV format. The purpose of this specific QUBE configuration is to describe the data structure and metadata of a dataset that contains information about marital and civil partnership status by category. 

Below is a line-by-line explanation of the different components of the mcps-new-context.json JSON document:

"$schema": "https://purl.org/csv-cubed/qube-config/v1" - This specifies the version of the QUBE schema being used. (Based on the $schema property here at the top of the configuration file, the context scheme used is defined by the URL https://purl.org/csv-cubed/qube-config/v1. This URL specifies the version 1 of the qube-config vocabulary, which is an open specification for metadata to describe data in CSV (Comma Separated Values) files.)

"title": "Marital and civil partnership status by category" - This is the title of the dataset.

"description": "Marital and civil partnership status by category" - This is a brief description of the dataset.

"creator": "https://www.gov.uk/government/organisations/office-for-national-statistics" - This is the organization that created the dataset.

"publisher": "https://www.gov.uk/government/organisations/office-for-national-statistics" - This is the organization that published the dataset.

"license": "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/" - This specifies the license under which the dataset is released.

"keywords": ["married", "partnership", "separated", "divorced", "widowed"] - These are keywords that describe the content of the dataset.

"columns": {...} - This section describes the columns of the dataset. There are four columns described in this configuration, which are "Lower Tier Local Authorities Code", "Lower Tier Local Authorities", "Marital and civil partnership status (12 categories) Code", and "Marital and civil partnership status (12 categories)".

"Lower Tier Local Authorities Code": {...} - This is a configuration for the first column of the dataset, which is called "Lower Tier Local Authorities Code". It specifies that the data for this column should be obtained from a "statistical-geography" template.

"Lower Tier Local Authorities": {...} - This is a configuration for the second column of the dataset, which is called "Lower Tier Local Authorities". It also specifies that the data for this column should be obtained from a "statistical-geography" template.

"Marital and civil partnership status (12 categories) Code": false - This is a configuration for the third column of the dataset, which is called "Marital and civil partnership status (12 categories) Code". It is set to false, which means that this column should not be included in the final dataset.

"Marital and civil partnership status (12 categories)": {...} - This is a configuration for the fourth column of the dataset, which is called "Marital and civil partnership status (12 categories)". It specifies that this column contains measures data, and defines the different categories of marital and civil partnership status that are included in the dataset.

"Observation": {...} - This section describes the data type of the dataset. It specifies that the data type is integer and provides information on the unit of measurement for the data.


The "definition_uri" is a field used to provide a URI (Uniform Resource Identifier) that defines the concept or category being described in the dataset. It is used to provide more information about the meaning of a specific data point or variable in the dataset.

In the given dataset, the "definition_uri" is used to define the 12 categories of marital and civil partnership status, providing a URI that defines the specific category. This allows for a more precise and standardized way of describing the categories, and also helps to ensure that the categories are understood consistently across different applications or contexts.

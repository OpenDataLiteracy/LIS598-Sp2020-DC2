# Data Curation II
This introductory chapter provides an overview of the conceptual content that we will engage in for DC II. The goal is to refresh our memory about concepts that were covered in DC I and how we will use these ideas throughout DC II.  

### Introduction
This class builds upon some foundational concepts and ideas that were introduced in Data Curation I. The emphasis of DC I was establishing some best (or good enough) practices for managing and preparing data for meaningful reuse. In introducing conceptual foundations in DC I, I also argued that practicing data curators need to acquire two types of knowledge: Declarative and Procedural. If you've taken a class with me you know that I think about this type of framework as being broadly useful for all types of learning. But, this framework is especially relevant for data curation.

To review: Procedural knowledge is *how* to do something, and declarative knowledge is knowing that something is the case. In other words, understanding something *about* the factual underpinnings of a concept. Less abstractly - lets use an example from our (now) everyday lives:  

**Declaratively** we know that a virus outbreak has certain distributions that are the direct result of collective action. If we take no action then there will be an increase in the rate of virus infections. But, if we collectively employ techniques like 'social distancing' then the infection rate will remain lower, essential services provided by public health workers will experience less of an impact, and society in general can effectively respond to incidents of viral infection. Over time we've started to refer to this as "flattening the curve" - that is taking collective action to decrease the height of a plotted distribution of infections over time.

[!](https://images.app.goo.gl/JxJ9EdamPZBqtRFu7)

**Procedurally** - How do we flatten a curve? Well, we employ techniques like social distancing, we wash our hands, we shut down broad sectors of the economy, we adhere to recommendations from the CDC, etc. It is only through knowing how to effectively combat viral outbreaks that we can put our declarative knowledge into practice.

Data curation is not so different from this example. We often need to first obtain some declarative knowledge about data and the ways way that it was collected, organized, and analyzed. Understanding the intricacies of these issues helps us to understand how we can design effective interventions. In other words, only after we obtain some declarative knowledge about data can we start to employ procedural techniques for preparing data to be managed and used effectively over time.

In DC I we focused a good deal of our time and effort on obtaining declarative knowledge. In DC II we start to tilt more strongly towards practicing and learning procedural techniques for putting this knowledge to work. In this course I will attempt to help you do this in two ways:
1. Deepening your declarative knowledge about data, management, organization, and encodings that are specific to the types of open data that we are able to reliably access and use via the web. By focusing in particular on open data we have the ability to practice with and use real world examples.
2. Exposing you to tools and strategies for employing these tools effectively in curating open data. Putting declarative knowledge to work takes practice, and it gets easier when we are able to abstract away from the particulars of any one context or any one tool's affordances (and limitations).

Before we begin diving into the content of DC II, it will help to revisit some definitions that were established in DC I:

**Data**: Data are various types of digital objects playing the role of evidence. Type and role distinctions have to do with the relational nature of data. A type is rigid (such as a file format) and a role is fluid (it can change given a context). A simple example will help make this clear: I am a person. This is a type. Regardless of any external circumstances I will remain a person. I am also a professor. This is a role that I play. I might, depending on the success of my tenure case, not be a professor in the future. This is simply a professional title that I have for a small amount of time. Data have similar rigid and fluid properties - A tabular dataset will have a type of structure (rows, columns, and values). Unless we take some purposeful action to transform this data it will remain tabular as a type. But, this tabular data might be evidence of some real world phenmena - it might be set of species occurrence records, the perciptation and temperature of a particular place, etc. This evidential role can shift and change depending on who is using the data, and for what purpose.

**Data curation**: Data curation is the active and ongoing management of data throughout a lifecycle of use, including its reuse in unanticipated contexts. This definition emphasizes that curation is not one narrow set of activities, but is an ongoing *process* that takes into account both material aspects of data, as well as the surrounding community of users that employ different practices while interacting with data and informaiton infrastructures.

**Metadata**: Metadata is most simply a set of standardized attribute-value pairs that provide contextual information about an object or artifact. Metadata, at an abstract level, has some features which are helpful for unpacking and making sense of the ways that descriptive, technical, and administrative information become useful for a digital object playing the role of evidence. Metadata can and often does include the following:  
- Classes -
- Sub-classes -
- Instances - are observations or concrete examples of a class. For example, my dog `Yael` is an instance of the sub-class Saluki. A Saluki is an instance of the sub-class Canine, which is an instance of a class of Mammals. A class or sub-class instance also has attributes or properties that define it is a member of that class or sub-class.
- Attributes - Are defining features of a class. An instance is a member of a class if it has all of the attributes of that class. For example, a Mammal has certain features (reproductive organs, respiratory system, etc) that define its base or necessary attributes for class membership.
- Relations - Instances and Classes can be related in one or many ways.

In DC I we also differentiated data and metadata based on its structure.

**Structured Metadata** Is quite literally a structured of attribute value pairs that are defined by a scheme. Most often, structured metadata is encoded in a machine readable format like XML or JSON. Crucially, structured metadata is compliant with and adheres to a standard that has defined attributes - such as Dublin Core, EML, DDI.

**Metadata Schema** Defines attributes (e.g. what do you mean by “creator” in ecology?); Suggests controls of values (e.g. dates = MM-DD-YYYY); Defines requirements for being “well-formed” (e.g. what fields Provide an implementation of the standard in an encoding are absolutely necessary for a valid metadata record?) (e.g. XML); and, Provides example use cases that are satisfied by the standard.

Structured metadata is, typically, differentiated by its documentation role.
- Descriptive Metadata: Tells us about objects, their creation, and the context in which they were created (Title, Author, Date)
- Technical Metadata: Tells us about the context of the data collection (Instrument, Computer, Algorithm)
- Administrative Metadata: Tell us about the management of that data (Rights statements, Provenance, etc. )

**Unstructured Metadata** is meant to provide contextual information that is Human Readable. This often takes the form of contextual information that records and makes clear how data were generated, how data were coded by creators, and relevant concerns that should be acknowledged in reusing these digital objects.

A further important distinction that we made about metadata is that it can be applied to both individual items, or collections or groups of related items. We referred to this as a distinction between **Item and Collection level metadata**.

**Expressivity Vs Tractability** The more expressive we make our metadata, the less tractable it is in terms of generating, managing, and computing for reuse. Inversely, if we optimize our documentation for tractability we sacifice some of the power in expressing information about attributes that define class membership. The challenge of all knowledge representation and organization activities - including metadata and documentation for data curation - is balancing expressivity and tractability.

**Normalization** Literally means making data conform to a normal schema. Practically, normalization includes the activities needed for transforming data structures, organizing variables (columns) and observations (rows), and editing data values so that they are consistent, interpretable, and match best practices in a field.

**Data Quality**: From the ISO 8000 definition we assume data quality are "...the degree to which a set of characteristics of data fulfills stated requirements.” In simpler terms this is the degree to which a set of data or metadata are fit for use. Examples of data quality characteristics include completeness, validity, accuracy, consistency, availability and timeliness.

### Summary 
These basic concepts give us some of the declarative knowledge we need to begin to do data curation work. Over the next ten weeks I will continue to offer working definitions about basic concepts related to DC II readings and topics. It's important to keep in mind these are "working definitions" - they may have important qualifications or need refinement in any particular context. The point of this long review isn't to ask you to memorize these concepts, but instead provide something like a 'term of reference' or knowledge base that we can continue to refine and improve over the course.    

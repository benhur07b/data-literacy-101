# Get
> How do I get the data from its source/location into my computer/machine?

Simply finding the data is not enough. Even if you know where to find the data, if you can’t get a hold of the data, it will be useless.

This step in the data pipeline involves getting the data from its initial location to your computer so that you can start working on it. This step can be short and easy or long and painful depending on variables such as data accessibility, availability, and the format that the data is in.

Your goal for this step is to get data in a [machine-readable](../open-data/machine-readable-data.md) format. This often requires preparation time, including the time needed to research and locate the appropriate tools for the task. **Very rarely will data just be magically available to analyze.**

```yaml remark
type: success
text: A common roadblock faced by people looking for data is the lack of disclosure of data owned by government agencies or public institutions. If there is no open data that is easily accessible then your first step would be to ask for the data nicely. However, that doesn't always work. When that is the case, it is important to know if there is a law in your country that guarantees Freedom of Information (FOI) that will allow you to make a formal request for the data that you seek.<br><br>It must be noted that even if an FOI request does not guarantee that you will get the data you seek, it is an important step that should not be ignored or forgotten.
```

## Things to consider
### Understanding key terms and technologies
It is important that you are at least familiar with terms such as: 
- **web scraping** - the automated retrieval information on a webpage
- **pdf extraction** - automatically extracting data tables from PDF 
- **OCR (optical character recognition)** - allows the extraction of texts from images or scanned documents
- **API (application programming interface)** - a way for people to query and request for information from a dataset/database

Even if your team does not have the skills to use these techniques or technologies, you should make yourself aware of them in order to avoid trying to do things manually (a very common mistake which is also very error-prone) instead of getting someone to help.
 

### Methods of getting data
If you are lucky and the data is readily available online in a digital format then you should be able to get the data directly. If not, you might need to request for the data or even extract the data from files and documents in order to convert them into a usable format. In the event that the data does not exist or you can't find sources for the data, you can do your own data collection.

**1. Get the data directly**
- downloading from open data portals
- using an Application Programming Interface (API) to access the data

**2. Request for the data**
- sending an FOI request or a formal request letter to the data owner

**3. Extract data from files and documents**
- extract tables from PDFs using applications such as [Tabula](https://tabula.technology/) or Excalibur
- scrape tables from webpages using Google Sheets, [webscraper.io](https://www.webscraper.io/), or programming with Python
- extracting texts from scanned documents or images using OCR

**4. Do the data collection yourself**
- Manual pen-and-paper surveys
- Using mobile data collection applicatiosn such as [ODK](https://getodk.org/)/[ODK-X](https://odk-x.org/), [KoBo](https://www.kobotoolbox.org/), or [Sabasi](https://sabasi.mobi/)
- Crowdsourcing via social media or platforms such as mTurk and samasource

### Data collection
Sometimes, no matter how hard you look, the data you need simply does not exist or is near impossible to find. When this is the case, you and your team may decide to collect the data yourselves. This data collection step can be simple or complex depending on the scope of the dataset that you want to build and the type of data needed.

For a quick reference on how to on mobile data collection, you can refer to: https://school-of-data.github.io/mobile-data-collection/index.html

## Common issues
### Bad data collection methodology
Data collection is often tricky to get right but doing it right—and doing it right the first time—is essential if you want to avoid delays and wasted effort.

There are two common types of data collection projects: 
- The first one is similar to a desk research where the goal is to create a dataset out of multiple data points from different sources. This is usually done online. 
- The other one involves field data collection and requires you to send people with questionnaires to fill either by themselves (e.g. doing rapid damage assessment after a disaster) or with the answers from a respondent. 

| **Type of project**    | **Common mistake**                                                                                                           | **Best practice**                                                                                                                                                        |
|------------------------|------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Online data collection | Starting with researching and collecting the data                                                                            | Defining the characteristics of the dataset you want to create (i.e. the columns of your spreadsheet)                                                                    |
| Online data collection | Not documenting the sources of the data                                                                                      | Creating a metadata file with the sources of all data; keeping untouched raw data in a separate folder                                                                   |
| Field data collection  | Inconsistency born from the lack of instructions given to staff about how to deal with responses outside of the expectations | Defining a process that covers all possibilities. This could mean including standard non-response categories such as ‘doesn’t know’ ‘no response’ ‘alternative response’ |
| Field data collection  | No anticipation of the analysis process in the methodology                                                                   | Defining the analysis questions (see module 2.1) ahead of time in order to understand how the data should be structured                                                  |

### No policy for data storage, access, and protection
No matter how large or how small the amount of data you need for a project, it is important that you idetify policies for the storage, access, and protection of the data. They do not need to be complex, but they should exist to will help ensure that you are prepared in case something bad happens with your data—e.g. accidental deletion, computers getting lost or not working, etc. This can include policies about data redundancy and backups (where and when is the data backed up), who has access to what data, and how to keep sensitive data such as personally-identifiable information private and secure.
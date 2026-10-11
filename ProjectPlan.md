Overview: 

Team:
  Arianna - in charge of understanding Datasets and completing Overview. Data visualization will be taken lead by Arianna, and we will generate more specific attributes to contribute to our definition of "accessibility".

  Anna - in charge of sending When to Meet to schedule bi-weekly meetings and discovering Gaps within our datasets. Anna will take lead in bringing up any issues that are of concern throughout our project. A constant "gut-check" is necessary for accuracy. 
  
  Sophie - in charge of understanding Constraints and consistently checking in on our project's limitations. Sophie will focus on editing the entire project to ensure consistency and accuracy throughout. 
  
  Amy - in charge of Timeline and ensuring team contributes equally and frequently. Also will take lead on analysis of project, fostering discussion amongst entire group on how to best utilize data efficiently to answer our Research Question. 

Research/Business Question: How can three different museums compare in terms of accessibility and the information they provide to the community?

Datasets:
1) https://github.com/NationalGalleryOfArt/opendata/tree/main/data
2) https://github.com/metmuseum/openaccess
3) https://github.com/art-institute-of-chicago/api-data

Timeline: (need to write out but this is rough outline)

- bi-weekly meetings and deadlines
- load in datas and understand information given in each dataset
- define what points of accessibility we want to focus on
- clean datasets separately to see overlapping data
- load in data to combined file
- organize data within combined file
- filter and reorganize to answer final question 

Datasets: In order to compare accessibility and information provided to the community across museums, we will use datasets from the National Gallery of Art (NGA), the Metropolitan Museum of Art (Met), and the Art Institute of Chicago (AIC). The NGA dataset consists of CSV files documented through a SQL-style data dictionary. We will use `objects.csv` for core object records (objectID, title, locationID, provenanceText), `locations.csv` and `preferred_locations.csv` for physical accessibility (publicAccess flags, site, room, public-facing descriptions), and `objects_constituents.csv` joined with `constituents.csv` for artist and donor relationships. `published_images.csv` adds image-level access through its `openaccess` flag and IIIF URLs. These files link via `objectID` and `locationID`.The Met provides only one CSV export containing all available fields. Columns we will use are `Object ID`, `Is Public Domain`, `Is Highlight`, `Department`, `Culture`, `Medium`, `Artist Display Name`, `Credit Line`, and `Link Resource`. This dataset demonstrates digital accessibility through public domain status, and shows cultural representation, but because it is a single flat file, comparisons are limited to columns within it. `Object ID` serves as its linking key. The AIC dataset is organized as folders of JSON files. We can use the `artworks` folder for object records and public domain status, `agents` for creator data, `galleries` for physical space information, `exhibitions` for programming context, `images` for image access and licensing, and `category-terms` for thematic classification. These link via `id`, with `gallery_id` and `image_id` connecting artworks to spaces and images. When used all together, these datasets can allow us to compare the physical accessibility (NGA locations, AIC galleries), digital accessibility (Met public domain, AIC image licensing, NGA open access), and content of cultural information (NGA provenance, Met cultural fields, AIC agent and exhibition data). Since these are separate institutions, we will mostly be comparing rather than concatenating the data. Object IDs link internal tables, while aggregate metrics enable cross-museum analysis of accessibility and community-facing information.


Constraints:

Gaps:

  Before making any more progress on this project there are a few gaps that need to be addressed about the datasets we chose and our analysis approach. First off, and most importantly, we need to define what accessibility means in terms of our research question. There are many different ways accessibility could be interpreted with respect to museums. For example, accessibility could refer to the ease of finding museum information online, the amount of information available about each art piece in the museum, or even the amount of accessibility features available in person at the museum. Also, we need to determine what specific information is available in each dataset that could be used to compare accessibility. There needs to be enough overlapping attributes present in each dataset, in order to make a correct comparison. This would also help our team determine how we will combine the data sets, as we need to find common attributes to correctly combine each dataset together for meaningful comparison. Finally, in order to make comparisons on accessibility, we need to standardize our comparison methods, to minimize bias in our data analysis. This includes how our team will deal with differences in dataset size and missing values. Overall, the next steps for this project is to address these gaps, so each team member is on the same page about what our project is addressing and our research goals. This will also ensure that we move forward with a standardized approach to our data analysis and cleaning.  


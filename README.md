# Vegan Recipe App Sitemap

```mermaid
flowchart TB
    Homepage --> Search
    Homepage --> Saved
    Homepage --> Profile
    Homepage --> OtherPages[Other Pages]
    OtherPages --> Contact
    OtherPages --> About
    Search --> RecipeDetail[Recipe Detail]
    Saved --> RecipeDetail
    Profile --> UserInformation[User Information]
    Profile --> Settings

    classDef rootNode fill:#4F3130,stroke:#AA5042,stroke-width:1px,color:#FFFFFF;
    classDef featureNode fill:#753742,stroke:#4F3130,stroke-width:1px,color:#FFFFFF;
    classDef innerNode fill:#AA5042,stroke:#753742,stroke-width:1px,color:#FFFFFF;
    classDef detailNode fill:#AA5042,stroke:#4F3130,stroke-width:1px,color:#FFFFFF;

    class Homepage rootNode;
    class Search,Saved,Profile,OtherPages featureNode;
    class Contact,About innerNode;
    class RecipeDetail detailNode;

# surfcamp-strapi
A surf camp landing page made using strapi

# Notes

- A page such as a landing page contains the hero section, info blocks etc. The data for that page is contained in a content type which has fields

- The content manager tab on the dashboard is used to add all of ours collections and content types to represent our data for out website

- In the content type builder we build all our new collection types and items	

- We can make a request from our Next.js app to our Strapi backend.
    - We first go to **Content Type Builder** and build a type in our case we made the single type called Home Page and gave it two fields, title and description.
    - Once we made this type, we went to **Content Manager** to add data, in our case we had boxes where we could give a title and description so we added Hello World and a description.
    - We then went to **Settings** > **Roles** > **Public** and exposed our end points so that we could call them using Postman and get the result. The result for hitting the /api/home-page endpoint was as follows:
```
{
    "data": {
        "id": 2,
        "documentId": "y2ai85vd0gjqobluxzwxosrc",
        "title": "Hello World",
        "description": "You are all awesome",
        "createdAt": "2026-01-01T06:50:15.659Z",
        "updatedAt": "2026-01-01T06:50:15.659Z",
        "publishedAt": "2026-01-01T06:50:15.673Z"
    },
    "meta": {}
}
```
- We can create reusable components using the Content Type Builder such as Logo which has attributes like logoText, image or Link component used in navigation bar. We can add attributes to them such as text, boolean

---
tags: []
---

# Models

## What 
A model contains common reusable information that can be referenced in your endpoint definitions or other models in your API design. The resources or endpoints in your API project might contain duplicate structures and response objects. Models reduce this duplication by helping you extract and define common resources making your project easier to maintain. 

## Best Practices 

### Avoid Cluttered APIs
When you have several endpoints with the same structure, objects, and properties, your API design is untidy. Ensure that you extract reusable artifacts and build them as pragmatic models referenced by other resources within your API project. 

### Use a Design First Approach
A design first approach helps create neat and consistent models. It will take longer, but it ensures you built an effective API that is easy to understand and maintain. 

## How to Create Models using the Stoplight Modeling Editor
1. [Create a new API project](/platform/projects/creating-a-project)
2. For this example we will be referring to endpoints created for a fictional Pet Store as listed below
- GET  /pets (return all pets)
- GET /pets{petid}  (return pet with  a specified id)
- POST / pets  (enter pet information)
- PUT  /pets{petid}  (update pet with a specified id)
- DELETE /pets{petid} (delete pet with a specified id)
3. The  GET  /pets method has an array of objects in the Response body with the following properties:

```
{ 
    id, (string),
    name, (string),
    date _created (string, date format),
    date_updated (string, date format),
    approved (Boolean),
    approved_by (string)
}
```

4. The  GET  /pets {petid} method duplicates the objects above  with the same properties:

```
{ 
    id, (string),
    name, (string),
    date _created (string, date format),
    date_updated (string, date format),
    approved (Boolean),
    approved_by (string)
}
```

5. The PUT / pets{petid}  method duplicates the object above in the Response body with a slight difference in the Request body which has the objects and properties below:
 
 ```
{ 
    id, string,
    approved boolean,
    approved_by string
}
```

<!-- theme:  info  -->
>Duplication of Objects: If you are required to make changes you would have to update this information in three or more endpoints. Creating a model solves this issue.

6. To create a model click on the + sign next to the Model section.

7. Enter the details for the key, title, and description fields

8. Click on the Editor Tab to create the object and specify the properties you want in the model (You can also copy and paste the JSON Schema from an endpoint into the Raw Schema section of the model)

9. Click the Save button to save the changes you have made in the editor 
10. Select the GET  /pets {petid} (or any endpoint)  and navigate to Responses→ Editor 
11. To reference the model in your endpoint, click on the object and select $ref as the array item type. Select the model you created from the drop down list


12. Select the Viewer section to see the changes you have made


13. All changes made to the properties of the object in the model are now automatically updated in all endpoints that make a reference to the model

# Recipe
```json
{
  "type": "object",
  "properties": {
    "id": { "type": "string" },
    "name": { "type": "string", "description": "Name of the recipe" },
    "description": { "type": "string", "description": "Brief description of the dish" },
    "prep_time": { "type": "string" },
    "cook_time": { "type": "string" },
    "servings": { "type": "string" },
    "ingredients": {
      "type": "array",
      "items": { "type": "string", "description": "e.g., '1 cup flour'" }
    },
    "instructions": {
      "type": "array",
      "items": { "type": "string", "description": "e.g., 'Preheat oven to 375F.'" }
    },
    "notes": { "type": "string", "description": "Optional tips or variations" },
    "createdAt": { "type": "string", "format": "date-time" }
  },
  "required": ["name", "ingredients", "instructions"]
}
```

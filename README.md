# The Sweet Shop App! 🍰
Welcome to the backend of Eni & Brenna's Flatiron Phase 1 project, which is an app for a future dessert shop!

**The Sweet Shop app** is an app for getting some feedback on our current dessert option contenders, and also getting some recommendations for other dessert ideas!

## How It Works

Our app is used to display the current dessert option contenders to the Sweet Shop, as well as get feedback for other dessert recommendations to be added to the shop's dessert list!

In order to get that information and have it update as needed, we have our backend JSON file to hold and organize the data. The JSON file contains two categories - desserts (that are to already be included in the Sweet Shop store), and recommendations (for desserts that could also be added to the Sweet Shop store in the future!).

### Current Dessert Options

The user will be able to click the dessert options button in order to see our current list of desserts. These are the desserts that are currently in line to be added to the store.

Each dessert contains the following data:

```
"desserts": [
    {
      "id": #,
      "name": "dessert name",
      "image": URL,
      "cost": #,
      "calories": #,
      "flavors": [
        "flavor1",
        "flavor2",
        "flavor3"
      ],
      "likes": #
    }
  ]
```

The user will be able to click the dessert options button in order to see our current list of desserts. These are the desserts that are currently in line to be added to the store, but we want to make sure we're including the ones people like the most!

The user will be able to click on each option in order to see additional dessert details, as well as a picture of the dessert. You will also be able to 'like' or 'dislike' the dessert.

If you see your favorite dessert, give it a 'like' (or *5*)!

If there's a dessert option that you absolutely don't think should be in there, feel free to give it a 'dislike'. We don't want to include any desserts that people don't want!

---

### Dessert Recommendations

Obviously, there's no way that our current dessert list includes everyone's favorite dessert, so we want to make sure we know what those other favorites might be! At the bottom of the app page, the user will be able to submit their own dessert recommendations to be added to the Sweet Shop, and we will get that posted data in our "recommendations" in the JSON file. We just need to know the type of dessert, the desired flavor, and then we also welcome any additional feedback comments too, which will then all be included in the JSON file (as well as any 'likes' that the recommendation has received):

```
 "recommendations": [
    {
      "id": #,
      "name": "dessert name",
      "flavor": "flavor",
      "comments": "user comments",
      "likes": #
    }
  ]
```
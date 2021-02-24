# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

📝 `NOTE` Paste this template at the top of your existing `README.md` file from part 1 of this assignment. (🚫 Remove this paragraph after after checking off completed user stories)

## Flix Part 2

### User Stories

#### REQUIRED (10pts)
- [x] (5pts) User can tap a cell to see more details about a particular movie.
- [x] (5pts) User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.

#### BONUS
- [x] (2pts) User can tap a poster in the collection view to see a detail screen of that movie.
- [ ] (2pts) In the detail view, when the user taps the poster, a new screen is presented modally where they can view the trailer.

### App Walkthrough GIF
`TODO://` Add the URL to your animated app walkthough `gif` in the image tag below, `YOUR_GIF_URL_HERE`. Make sure the gif actually renders and animates when viewing this README. (🚫 Remove this paragraph after after adding gif)

<img src="http://g.recordit.co/q28BTUNRsE.gif" width=250><br>

### Notes
- I had issues with the backdrop image overlapping the poster image in my details screen. I just repositioned the image views to resolve this.
- I noticed some movies (like The Flash (2022) and The Flash (1990)) had no backdrops which would cause crashes. I resolved this issue by changing 'let backdropPath = movie["backdrop_path"] as! String' to 'let backdropPath = (movie["backdrop_path"] as? String) ?? "0"' .

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [ ] (1pt) Run your app on a real device.

### App Walkthrough GIF

<img src="http://g.recordit.co/ZESutUQhSK.gif" width=250><br>

### Notes
- My Mac runs on the M1 chip and I ran into some issues with installing CocoaPods. A few lines in the terminal solved my issue.
- I'm simulating my app with the iPhone 12 and my launch screen image was shifted to the side. I had to reposition it since my storyboard was being viewed as an iPhone 11 Pro.

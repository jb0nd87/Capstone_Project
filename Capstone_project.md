# Project Overview

## Project Links

- [Link to github repo]()
- [Netlify link]()

## Project Description

An rock climbers help app that will show the national park in the U.S. where climbing is allowed. It will be built using D3 for the visualizations and using Google Maps API. I can be used to track which places the user has been and which climbs they have done and be able to mark them down as completed.

- [Marvel Site](https://www.marvel.com/comics?&options%5Boffset%5D=0&totalcount=12)

## API



## Wireframes

Here are my wireframes for how I would like the finished app to look like.

- [Wireframes]()
- [React Architecture]()
- [Time/Priority Matrix]()

### MVP/PostMVP - 5min

<!-- The functionality will then be divided into two separate lists: MPV and PostMVP.  Carefully decided what is placed into your MVP as the client will expect this functionality to be implemented upon project completion.   -->

#### MVP

- Find an use external api
- Render data on page
- Allow user to interact with the page

#### PostMVP EXAMPLE

- Add localStorage or firebase for storage

## Components

##### Writing out your components and its descriptions isn't a required part of the proposal but can be helpful.

Based on the initial logic defined in the previous sections try and breakdown the logic further into stateless/stateful components.

| Component    |                          Description                          |
| ------------ | :-----------------------------------------------------------: |
| App          | This will make the initial data pull and include React Router |
| Header       |          This will render the header include the nav          |
| Comic        |          This will show the first comic on the page           |
| Comic Filter |         This will render the Comic Cards in the body          |
| Footer       |          This will render the header include the nav          |

<!-- Time frames are also key in the development cycle.  You have limited time to code all phases of the game.  Your estimates can then be used to evalute game possibilities based on time needed and the actual time you have before game must be submitted. It's always best to pad the time by a few hours so that you account for the unknown so add and additional hour or two to each component to play it safe. Also, put a gif at the top of your Readme before you pitch, and you'll get a panda prize. -->

| Component    | Priority | Estimated Time | Time Invested | Actual Time |
| ------------ | :------: | :------------: | :-----------: | :---------: |
| App          |    H     |     10hrs      |     6hrs      |    10hrs    |
| Header       |    M     |      3hrs      |     2hrs      |    4hrs     |
| Comics       |    H     |     10hrs      |     10hrs     |    12hrs    |
| Comic Filter |    H     |     10hrs      |      hrs      |    8hrs     |
| Footer       |    L     |      3hrs      |     3hrs      |    3hrs     |
| Total        |    H     |     36hrs      |     31hrs     |    37hrs    |

## Additional Libraries

I used react bootstrap for my navbar.

## Code Snippet

The thing that got me the most excited was when I got the .map function to work and return data with the help of Joe and also another friend of mine.

```
const Comics = (props) => {
	// const [comicAPIResults, setComicAPIResults] = useState([]);
	console.log('comics', props.comicData);
	const renderComicData = () => {
		return props.comicData
			? props.comicData.map((comic) => {
					return <ComicInfo comicData={comic} />;
			  })
			: '';
	};
	return <>{renderComicData()}</>;
};

export default Comics;

```

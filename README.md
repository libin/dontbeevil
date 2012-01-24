# focus on the user

How much better would social search be if Google surfaced results from all across the web? The results speak for themselves. We created a tool that uses Google’s own relevance measure—the ranking of their organic search results—to determine what social content should appear in the areas where Google+ results are currently hardcoded.

All of the information in this demo comes from Google itself, and all of the ranking decisions are made by Google's own algorithms. No other services or APIs are accessed.

## How It Works
When you search for "cooking" today, Google decides that renowned chef Jamie Oliver is a relevant social result. That makes sense. But rather than linking to Jamie's Twitter profile, which is updated daily, Google links to his Google+ profile, which was last updated nearly two months ago. Is Google's relevance algorithm simply misguided?

No. If you search Google for Jamie Oliver directly, his Twitter profile is the first social result that appears. His abandoned Google+ profile doesn't even appear on the first page of results. When Google's engineers are allowed to focus purely on relevancy, they get it right.

So that's what our "bookmarklet" does. It looks at the three places where Google only shows Google+ results and then automatically googles Google to see if Google finds a result more relevant than Google+.

For more info, read [focus on the user](http://www.focusontheuser.org/).

This proof of concept was built by some engineers at Facebook, Twitter and MySpace, in consultation with several other social networking companies. We are open-sourcing the code so that anyone may use it or make it even better.

Contact us at team@focusontheuser.org
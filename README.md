## Nature 101
============

This is a map aimed to help families connect to nature in San Francisco. Rather than piling on lots of loayers and data, we're trying an intentionally simpler approach. Pick a top five in just three categories and present those in a visually compelling way with short, chatty text.

This map uses a set of CartoDB map visualizations combined with [Odyssey.js](https://cartodb.github.io/odyssey.js/) to create a curated tour of great places to experience nature with kids in San Francisco.

The map is served using Github Pages, so we've set the default branch to `gh-pages`. For our map, the CartoDB visualizations are hosted at https://sfnaturemaps.cartodb.com ([here's an example map](https://sfnaturemaps.cartodb.com/viz/988fdb2e-eaf1-11e5-8daa-0ecfd53eb7d3/public_map)), and the core narrative content is contained in a block of markdown on [these lines in `index.html`](https://github.com/GreenInfo-Network/sfnaturemaps/blob/gh-pages/index.html#L490-L674).

This is intentionally a very lightwieght solution. If you wanted to adapt to your own story, just create one or more CartoDb maps and get the `viz.json` links (by accessing the API tab under "Publish"). Those get swapped into the `viz.json: ` parameters, [like this](https://github.com/GreenInfo-Network/sfnaturemaps/blob/gh-pages/index.html#L495).

Then edit the markdown text elements, image links and centerpoints to showcase other places and stories.
The three categories (wild life, wild lands, and wild rides) came out of a series of focus groups in 2015, so we think they're solid and any city could make a great map with justthose three elements. But if you want to change those, dig into `Odyssey_GIN.js` with four find-replace and have at it ([here's an example line](https://github.com/GreenInfo-Network/sfnaturemaps/blob/gh-pages/Odyssey_GIN.js#L974). 

This was developed by [GreenInfo Network](http://greeninfo.org) in 2016, in collaboration with sfnaturemaps.org and with funding from the SEED Foundation.

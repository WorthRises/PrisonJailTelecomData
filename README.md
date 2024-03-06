# #ConnectFamiliesNow Public Datasets

For more background on the #ConnectFamiliesNow organizing, visit our [website](https://connectfamiliesnow.com/).
To see a a heatmap representation of the current datsets, visit the [prison telecom data project](https://connectfamiliesnow.com/data?noredirect).

## The Data

You can download the CSV's with the latest rate data [here](https://github.com/blueshift-tech/worth-rises/tree/main/07-20-22).

To save a file: click on any file with a `.csv` extension, and in the upper right-hand corner, select "Copy raw contents". You can then paste into a Google Sheet, text file, or Excel. Or, from the upper right-hand menu, select "Raw", which takes you to a url ending in `.csv`. Use "Command + S" while viewing this page to save this file as a `.csv` extension.

The folders above represent the date when data was collected. Select a folder to view prices for a 15 minute phone call for prison inmates at state, county, and local level facilities.

The datasets contain rate information pulled from the three major telecom vendors in the prison industry: ICSolutions, ViaPath (formerly GTL), and Securus. These rates are reported at a facility level, before we classify each facility according to agency (either state, county, local, or other). Rates are then grouped according to agency, so prices reflect a state, county, or local geography.

Telecom vendors sign contracts at the agency level, so we can group prices according to agency and find consistent price values. There were some outliers to this trend, where an agency had a vast majority of prices listed at one value with a limited few at a second value. The few with a second conflicting value were treated as outliers and removed from the dataset.

If multiple vendors reported a contract with a single agency, we confirmed the agency's telecom vendor either through their website, or via phone call if no information was publicly available.

There is also a known subset of counties that send inmates to regional or state facilities, and thus have no county-level facility in the initial dataset. These counties are added to the final dataset with a county-level agency classification, where the corresponding regional or state-level facility prices are copied for each county. This way, we can see the price that an inmate will pay if they are processed by any of these counties.

Both in-state and out-of-state rates are collected and reported in the final datasets.

## Notes
Because this data is scraped from private entities, it is updated and ammended on a schedule we do not control. Our data represents telecom rates as those entities report them publicly.

ViaPath data after February 23, 2024 is corrected to account for a rounding error in the 1-minute prices posted on the ViaPath website. Data listed before February 23, 2024 for jurisdictions served by ViaPath could not be corrected, and might include minor inaccuracies resulting from extrapolation of 15-minute call price from rounded 1-minute price. 

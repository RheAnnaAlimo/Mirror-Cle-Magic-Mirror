```JavaScript
 language: "en",
        timeFormat: 12,
        units: "imperial",
        
  modules: [
                {
                        module: "alert",
                },
                {
                        module: "updatenotification",
                        position: "top_bar"
                },
                {
                        module: "clock",
                        position: "top_left"
                },
                {
                        module: "calendar",
                        header: "US Holidays",
                        position: "top_right",
                        config: {
                                calendars: [
                                        { symbol: "calendar-check-o ",
                                                url: "webcal://www.calendarlabs.com/templates/ical/US-Holidays.ics"

                                        }
                                ]
                        }
                },
                {
                        module: "compliments",
                        position: "upper_third"
                },
                {
                        module: "currentweather",
                        position: "top_right",
                        config: {
                                location: "Temecula, CA",
                                locationID:"5401395",  //ID from http://bulk.op$
                                appid: "c75790f0513d8be233f8083226fe8642" //This is my personal appid
                        }
                },
        //      {
        //              module: "weatherforecast",
        //              position: "top_right",
        //              header: "Weather Forecast",
        //              config: {
        //                      location: "Temecula, CA",
        //                      locationID: "5401395",  //ID from http://www.openweathermap.org/help/city_list.txt
        //                      appid: "c75790f0513d8be233f8083226fe8642"
        //              }
        //      },
                {
                        module: "newsfeed",
                        position: "bottom_bar",
                        config: {
                                feeds: [
                                        {
                                                title: "New York Times",
                                                url: "http://www.nytimes.com/services/xml/rss/nyt/HomePage.xml"
                                        }
                                ],
                                showSourceTitle: true,
                                showPublishDate: true
                        }
                },
                {
                        module: 'stocks',
                        position: 'bottom_right',
                        config: {
                                stocks: 'MSFT,GOOG,INTC,TSLA,FB,NFLX,AMZN,IBM', // stock symbols
                                updateInterval: 37000 // update interval in milliseconds
                                }
                },
        ]
};

```


Original configuration by Michael Teeuw http://michaelteeuw.nl
 * MIT Licensed.

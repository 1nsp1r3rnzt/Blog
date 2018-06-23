---
permalink: /about/
title: "About us"
layout: single
author_profile: true
---

Hey There, I am Ranjit Singh, a graduate of Carleton University. 

> This blog is playground for my Programming journey as I believe that we don't understand anything until we learn it more than one way.

I write about programming mostly [Android development](/categories/android/), [automation](/tags/automation/), [book summaries](/books) and [Reviews](/categories/reviews/).
I take notes of my [favourite podcasts](/podcasts/).

## SkillSet
I am on a quest to improve skillset. Here is the comparision.       
<canvas id="radar-chart" width="600" height="800"></canvas>
<script>
    var notations = {
        0:"",
        1:"no",
        20:"Theory",
        50:"proficient",
        70:"Great",
        90:"outstanding",
            }

    new Chart(document.getElementById("radar-chart"), {
        type: 'radar',
        
        data: {
            labels: ["GNU/Linux", "Android Development", "Core Java", "Frontend HTML/CSS", "UI / UX", "Blogging", "Database", "Javascript", "Windows", "CMS(Wordpress)"],
            datasets: [{
                label: "2017",
                fill: true,
                backgroundColor: "rgba(51,133,255,0.2)",
                borderColor: "rgba(51,133,255,1)",
                pointBorderColor: "#fff",
                pointBackgroundColor: "rgba(51,133,255,1)",
                data: [33, 49, 50, 67, 39, 80, 60, 50, 90,80]
            }, {
                label: "2018",
                fill: true,
                backgroundColor: "rgba(255,99,132,0.2)",
                borderColor: "rgba(255,99,132,1)",
                pointBorderColor: "#fff",
                pointBackgroundColor: "rgba(255,99,132,1)",
                pointBorderColor: "#fff",
                data: [60, 67, 80, 68, 50, 90, 80, 60, 90,81]
            }]
        },


        options: {
            scale: {
                responsive: true,
                ticks: {
                    display: true,
                    min:0,
                    beginAtZero: true,
                    max: 100, 
                    userCallback: function (value, index, values) {
                        if( typeof notations[value]!="undefined")
                        {
                             return notations[value];
                         }
                    else {
                      return value;
                           }

                },
                },

                gridLines: {
                    display: true,
                    color: [
                        "rgba(245, 245,220,1)",
                        "rgba(0, 0,255,0.1)",
                        "rgba(165, 42,42,0.1)",
                        "rgba(0, 255,255,0.1)",
                        "rgba(0, 0,139,0.3)",
                        "rgba(0, 139,139,0.1)",
                        "rgba(169, 169,169,1)",
                        "rgba(0, 100,0,0.1)",
                        "rgba(189, 22,107,0.1)",
                        "rgba(139, 0,139,0.1)",
                        "rgba(139, 0,139,0.1)",
                        "rgba(139, 0,139,0.1)",


                    ], 
                },

                angleLines: {
                    display: true,
                    color: "red",
                },
                pointLabels: {
                    // callback: function(value, index, values) {
                    //     return '$' + value;
                    // }
                    fontColor: '#' + Math.random().toString(16).slice(2, 8).toUpperCase(),
                },
            },
            legend: {
                display: true
            },
            title: {
                display: false,
                // text: 'Skill Set'
            },
        }
    });
</script>



##  *Contact me*
I love intelligent conversations about solving real-world problems through programming and technology.
 You can reach me at [Twitter](https://twitter.com/king99immortal) or [Linkedin](https://ca.linkedin.com/in/ranjitsinghsaini) 


## Resources

Here are some resources you might find useful.

[Best Google Chrome extensions of 2017 for web devs to enhance productivity](/best-google-chrome-extensions/)
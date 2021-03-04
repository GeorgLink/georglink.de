---
id: 737
title: How to measure the impact of your open source project
date: 2018-11-29T16:50:45-06:00
author: Georg Link
layout: revision
guid: http://www.georglink.de/2018/11/29/734-revision-v1--737
permalink: /2018/11/29/734-revision-v1--737
---
We published this article [originally on Opensource.com](https://opensource.com/article/18/5/metrics-project-success).

This article was co-authored by Vinod Ahuja, Don Marti, Georg Link, Matt Germonprez, and Sean Goggins.

> Conventional metrics of open source projects lack the power to predict their impact. The bad news is, there is no significant correlation between open source activity metrics and project impact. The good news? There are paths forward.
> 
> Let&#8217;s start with some questions: How do you measure the impact of your open source project? What value does your project provide to other projects? How is your project important within an open source ecosystem? Can you predict your project&#8217;s impact using open source metrics that you can follow day to day?
> 
> If these questions resonate, chances are you care about measuring the impact of your open source project. On Opensource.com, we have already learned about measuring the <a href="https://opensource.com/bus/16/8/measuring-community-health" target="_blank" rel="noopener">project’s health</a>, the <a href="https://opensource.com/open-organization/15/6/measuring-community-manager-performance" target="_blank" rel="noopener">community manager’s performance</a>, the <a href="https://opensource.com/article/17/9/prospector-chaoss" target="_blank" rel="noopener">tools available for measuring</a>, and the <a href="https://opensource.com/business/16/9/choosing-right-metrics" target="_blank" rel="noopener">right metrics to use</a>—and we understand that <a href="https://opensource.com/business/16/7/measuring-what-matters" target="_blank" rel="noopener">not all metrics are to be trusted</a>.
> 
> While all these factors are critical in building a comprehensive picture of open source project health, there is more to the story. Indeed, many metrics fail to provide the information we need in a timely fashion. We want to use <a href="http://www.information-age.com/companies-wasting-millions-digital-investment-123471707/" target="_blank" rel="noopener">predictive metrics</a> on a daily basis—metrics that are correlated with, and that act as predictors of, the outcomes and impact metrics that we care about.
> 
> Most open source project metrics focus on project metadata, such as contributor and commit counts, without addressing whether the project impacts a broader open source ecosystem. Unfortunately, a project that has a great number of contributors and an active flow of contributions may not be, and might never be, relevant to other projects in an open source ecosystem. To better understand the impact of a project, it is important to consider the broader context of an open source ecosystem. This article introduces the V-index as a measure of impact (see <a href="https://digitalcommons.unomaha.edu/isqafacpub/62/" target="_blank" rel="noopener">Regression Analysis of Open Source Project Impact: Relationships with Activity and Rewards</a>).
> 
> ## Who cares about project impact?
> 
> Sponsors of open source projects care about their impact. A foundation that&#8217;s hosting an open source project likely wants it to be widely used, for example, or an organization that&#8217;s paying developers to work on a project will want to ensure that their efforts are making a difference. Consequently, software developers or project managers may need to use metrics to make the case that the time and effort spent on an open source project is creating real value for their employer.
> 
> Open source project members also care about the impact of their project. High-impact projects can be a source of pride and motivation for developers. Within the open source ecosystem, it means that people are interested in new development and ready to report bugs. High impact means that projects need the code base to be maintained and vulnerabilities to be addressed, which is an incentive to support project members.
> 
> ## Open source project impact
> 
> An effective way to understand an open source project’s impact is through its software libraries. A software library certainly impacts the projects in which it is used, and popular libraries have also changed the way software is developed by providing functionality across a variety of software projects.
> 
> For example, the <a href="https://getbootstrap.com/" target="_blank" rel="noopener">Bootstrap library</a> revolutionized website interfaces and has become a de facto standard. But Bootstrap depends on another widely used library: <a href="https://jquery.com/" target="_blank" rel="noopener">jQuery</a>. jQuery simplifies the use of JavaScript in website development. The impact of jQuery on Bootstrap, and on web development as a whole, cannot be overstated, and this impact is evident in the library dependency relationship between the two.
> 
> The jQuery/Bootstrap example demonstrates how software libraries can have an impact. Within the open source ecosystem, jQuery is an upstream project to Bootstrap, which itself is an upstream project to many websites and web frameworks, as shown below:
> 
> <div class="content">
>   <p>
>     <div id="attachment_735" style="width: 310px" class="wp-caption aligncenter">
>       <a href="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1.png"><img aria-describedby="caption-attachment-735" loading="lazy" class="size-medium wp-image-735" src="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1-300x300.png" alt="downstream depedency depiction for jQuery and Bootstrap" width="300" height="300" srcset="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1-300x300.png 300w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1-150x150.png 150w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1-768x768.png 768w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1-1024x1024.png 1024w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-1.png 1108w" sizes="(max-width: 300px) 100vw, 300px" /></a>
>       
>       <p id="caption-attachment-735" class="wp-caption-text">
>         Figure 1: An open source project dependency within an open source ecosystem: The jQuery project is the upstream project to Bootstrap and many other projects, which themselves may be upstream to more projects. (Graphic by Kevin M. Lumbard, licensed CC-BY-SA-3.0. River delta background by Messer Woland, licensed CC-BY-SA-3.0. Logos are property of respective right owners.)
>       </p>
>     </div>
>   </p>
> </div>
> 
> <div class="media media-element-container media-default media-wysiwyg-align-center">
>   <div id="file-397431" class="file file-image file-image-png">
>     <div class="content">
>       <div class="field field-name-field-file-image-caption field-type-text-long field-label-hidden">
>         <div class="field-items">
>           <div class="field-item even">
>             <p class="rtecenter">
>               </div> </div> </div> </div> </div> </div> 
>               
>               <h2>
>                 Measuring impact
>               </h2>
>               
>               <p>
>                 Many metrics are being developed to measure the impact of an open source project. These include the number of users, downloads, installs, mentions in media (e.g., blogs, news, YouTube videos, and job postings), the availability of commercial offerings, and the number of add-on products. But such metrics isolate impact within that specific project and don’t fully demonstrate the impact of a software library within an open source ecosystem.
>               </p>
>               
>               <p>
>                 To measure the impact of an open source project within the open source ecosystem, let&#8217;s borrow a metric from academia: the <a href="https://en.wikipedia.org/wiki/H-index" target="_blank" rel="noopener"><em>h</em>-index</a>. This determines the impact of an author through the relationship of how many publications he or she has produced, and how many other authors have cited these publications. We propose, therefore, that a project’s impact in an open source ecosystem can be determined by downstream dependencies (i.e., how many downstream open source projects use them and how often those downstream projects are themselves used).
>               </p>
>               
>               <h2>
>                 V-index
>               </h2>
>               
>               <p>
>                 A downstream dependency exists when a software library is used within another piece of software. The V-index, which encapsulates our proposed measure of impact, is the maximum number of first-order downstream dependencies that themselves have at least an equal number of second-order downstream dependencies. The first-order dependency is the number of open source projects that use the library. The second-order downstream dependency is determined by how often a first-order dependent project is used within other open source projects.
>               </p>
>               
>               <p>
>                 The V-index is elaborated in three different scenarios:
>               </p>
>               
>               <table border="1" width="624" frame="VOID" rules="GROUPS" cellspacing="0" cellpadding="7">
>                 <colgroup> <col width="87" /></colgroup> <colgroup> <col width="87" /> <col width="4369" /> <col width="84" /></colgroup> <colgroup> <col width="84" /> <col width="4369" /> <col width="85" /> <col width="85" /></colgroup> <tr valign="TOP">
>                   <td colspan="2" width="189" height="15">
>                     <p align="CENTER">
>                       <span style="font-size: small;"><b>Scenario A</b></span>
>                     </p>
>                   </td>
>                   
>                   <td width="4369">
>                     <p align="CENTER">
>                       </td> 
>                       
>                       <td colspan="2" width="182">
>                         <p align="CENTER">
>                           <span style="font-size: small;"><b>Scenario B</b></span>
>                         </p>
>                       </td>
>                       
>                       <td width="4369">
>                         <p align="CENTER">
>                           </td> 
>                           
>                           <td colspan="2" width="184">
>                             <p align="CENTER">
>                               <span style="font-size: small;"><b>Scenario C</b></span>
>                             </p>
>                           </td></tr> 
>                           
>                           <tr valign="TOP">
>                             <td width="87" height="30">
>                               <span style="font-size: small;"><b>First-order dependencies</b></span>
>                             </td>
>                             
>                             <td width="87">
>                               <span style="font-size: small;"><b>Second-order dependencies</b></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;"><b>First-order dependencies</b></span>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;"><b>Second-order dependencies</b></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="85">
>                               <span style="font-size: small;"><b>First-order dependencies</b></span>
>                             </td>
>                             
>                             <td width="85">
>                               <span style="font-size: small;"><b>Second-order dependencies</b></span>
>                             </td>
>                           </tr>
>                           
>                           <tr valign="TOP">
>                             <td width="87" height="15">
>                               <span style="font-size: small;">Dependency 1</span>
>                             </td>
>                             
>                             <td width="87">
>                               <span style="font-size: small;"></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">Dependency 1</span>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">4</span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="85">
>                               <span style="font-size: small;">Dependency 1</span>
>                             </td>
>                             
>                             <td width="85">
>                               <span style="font-size: small;">40</span>
>                             </td>
>                           </tr>
>                           
>                           <tr valign="TOP">
>                             <td width="87" height="15">
>                               <span style="font-size: small;">Dependency 2</span>
>                             </td>
>                             
>                             <td width="87">
>                               <span style="font-size: small;"></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">Dependency 2</span>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">4</span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                           </tr>
>                           
>                           <tr valign="TOP">
>                             <td width="87" height="15">
>                               <span style="font-size: small;">Dependency 3</span>
>                             </td>
>                             
>                             <td width="87">
>                               <span style="font-size: small;"></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">Dependency 3</span>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">4</span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                           </tr>
>                           
>                           <tr valign="TOP">
>                             <td width="87" height="15">
>                               <span style="font-size: small;">Dependency 4</span>
>                             </td>
>                             
>                             <td width="87">
>                               <span style="font-size: small;"></span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">Dependency 4</span>
>                             </td>
>                             
>                             <td width="84">
>                               <span style="font-size: small;">4</span>
>                             </td>
>                             
>                             <td width="4369">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                             
>                             <td width="85">
>
>                             </td>
>                           </tr>
>                           
>                           <tr valign="TOP">
>                             <td colspan="2" width="189" height="75">
>                               <p align="JUSTIFY">
>                                 <span style="font-size: small;"><b>Project A has a V-index of 0.</b></span>
>                               </p>
>                               
>                               <p align="JUSTIFY">
>                                 <span style="font-size: small;">The project has four projects that depend on it. No other project depends on these projects. </span><span style="font-size: small;">The V-index of Project A is 0 because zero first-order dependencies have any second-order dependencies.</span>
>                               </p>
>                             </td>
>                             
>                             <td width="4369">
>                               <p align="JUSTIFY">
>                                 </td> 
>                                 
>                                 <td colspan="2" width="182">
>                                   <p align="JUSTIFY">
>                                     <span style="font-size: small;"><b>Project B has a V-index of 4. </b></span>
>                                   </p>
>                                   
>                                   <p align="JUSTIFY">
>                                     <span style="font-size: small;">The project has four projects that depend on it. Each of these projects has four projects that depend on them. The V-Index of Project B is four because each of the four first-order dependencies have at least four second-order dependencies.</span>
>                                   </p>
>                                 </td>
>                                 
>                                 <td width="4369">
>                                   <p align="JUSTIFY">
>                                     </td> 
>                                     
>                                     <td colspan="2" width="184">
>                                       <p align="JUSTIFY">
>                                         <span style="font-size: small;"><b>Project C has a V-index of 1. </b></span>
>                                       </p>
>                                       
>                                       <p align="JUSTIFY">
>                                         <span style="font-size: small;">The project has one project that depends on it. This project has 40 projects that depend on it.</span> <span style="font-size: small;">The V-Index of Project C is 1 because it has one first-order dependency that has at least one second-order dependency.</span>
>                                       </p>
>                                     </td></tr> </tbody> </table> 
>                                     
>                                     <p>
>                                       Looking at a practical example, jQuery has a V-index of 98. It has 13,848 first-order dependencies, of which Bootstrap is one, with 5,005 second-order dependencies. Of the 13,848, only 98 first-order dependencies have 98 or more second-order dependencies, as shown below:
>                                     </p>
>                                     
>                                     <div class="media media-element-container media-default">
>                                       <div id="file-397436" class="file file-image file-image-png">
>                                         <div class="content">
>                                           <p>
>                                             <div id="attachment_736" style="width: 310px" class="wp-caption aligncenter">
>                                               <a href="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-2.png"><img aria-describedby="caption-attachment-736" loading="lazy" class="size-medium wp-image-736" src="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-2-300x218.png" alt="V-Index graphical depiction" width="300" height="218" srcset="http://www.georglink.de/media/2018/11/ahuja-metrics-fig-2-300x218.png 300w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-2-768x559.png 768w, http://www.georglink.de/media/2018/11/ahuja-metrics-fig-2.png 920w" sizes="(max-width: 300px) 100vw, 300px" /></a>
>                                               
>                                               <p id="caption-attachment-736" class="wp-caption-text">
>                                                 Figure 2: V-index of jQuery: The x-axis represents the downstream open source projects (first-order downstream dependencies) sorted by the number of their own downstream dependencies. The y-axis represents the number of downstream dependencies of each first-order open source project on the x-axis (second-order downstream dependencies). The V-index is the number of first-order downstream dependencies that have at least the same number of second-order downstream dependencies. (Graphic by Kevin M. Lumbard, licensed CC-BY-SA-3.0. Logos are property of respective right owners.)
>                                               </p>
>                                             </div>
>                                           </p>
>                                           
>                                           <div class="field field-name-field-file-image-caption field-type-text-long field-label-hidden">
>                                             <div class="field-items">
>                                               <div class="field-item even">
>                                                 <p class="rtecenter">
>                                                   </div> </div> </div> </div> </div> </div> 
>                                                   
>                                                   <h2>
>                                                     Increase impact with new metrics
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     How do you increase your open source project&#8217;s impact? Well, you need to convince other projects to use your project. Unfortunately, there is no single activity that will make this happen. However, there are steps you can take to make a project impactful, and there are ways to measure how well you do them. Let’s look at which of these measures are correlated with impact.
>                                                   </p>
>                                                   
>                                                   <p>
>                                                     We summarize the findings below based on previous <a href="https://digitalcommons.unomaha.edu/isqafacpub/62/" target="_blank" rel="noopener">correlation analysis</a>. The correlation analysis used a sample of metrics for <a href="https://blog.zgp.org/three-kinds-of-open-source-metrics/" target="_blank" rel="noopener">three kinds of open source metrics</a>:
>                                                   </p>
>                                                   
>                                                   <ol>
>                                                     <li>
>                                                       <i>Activity metrics</i> measure metadata such as contributor or commit counts. Project contributors can increase these metrics by doing more work on the project and getting more people involved.
>                                                     </li>
>                                                     <li>
>                                                       <i>Reward metrics</i> measure how well the project is meeting contributor’s expectations. They may improve with faster acceptance of contributions.
>                                                     </li>
>                                                     <li>
>                                                       <i>Impact metrics</i> measure the impact on users and other projects.
>                                                     </li>
>                                                   </ol>
>                                                   
>                                                   <p>
>                                                     The V-index was developed to measure impact metrics. The correlation was tested for 604 projects that were started in 2014 or 2015, that used the <a href="https://www.rust-lang.org/en-US/" target="_blank" rel="noopener">Rust programming language</a>, that were listed in GHTorrent and Libraries.io (the data sources), and that had at least one downstream dependency.
>                                                   </p>
>                                                   
>                                                   <p>
>                                                     The findings show that none of the conventional open source activity metrics correlate with impact. This lack of predictive activity metrics means that we have no good predictors to manage our open source projects.
>                                                   </p>
>                                                   
>                                                   <p>
>                                                     Does this mean all is lost? We think not. Several open source projects are building next-generation metrics that project sponsors, maintainers, and downstream users might be able to rely on in the future. Here are four paths to finding the predictive metrics we need to boost the impact of our open source projects:
>                                                   </p>
>                                                   
>                                                   <h2>
>                                                     1. Add software quality metrics
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     The first idea is to combine open source activity metrics with conventional software engineering metrics, such as code coverage. Conventional open source activity metrics focus heavily on the development dynamics within the project. The focus on activity metrics excludes software quality factors, which might be more important for people choosing a software library. Conventional open source activity metrics make it difficult to distinguish productive activity from unproductive activity. Combining a software engineering metric with an open source activity metric could make the latter more valuable.
>                                                   </p>
>                                                   
>                                                   <h2>
>                                                     2. Understand the user community
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     The second idea involves using natural language processing to determine the sentiment within an open source project, especially where users of the software participate. Conventional open source activity metrics rely only on metadata. Knowing the number of interactions does not help us understand the quality and substance of community. <a href="https://github.com/sagesharp/foss-heartbeat" target="_blank" rel="noopener">FOSS Heartbeat</a>, while currently not maintained, offers a solution.
>                                                   </p>
>                                                   
>                                                   <h2>
>                                                     3. Market mechanisms
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     The third idea is to draw a connection between impact and the value of a software library. Existing valuation methods focus on the project itself (i.e., <a href="https://blog.quenda.co/posts/hurts-of-code">development costs</a>) rather than the value others derive from it. A problem that open source faces is the absence of price signals that can inform the value users receive from a software library. To draw a connection between impact and value, we need new market mechanisms, like the ones proposed by <a href="https://bugmark.net/" target="_blank" rel="noopener">Bugmark</a>.
>                                                   </p>
>                                                   
>                                                   <h2>
>                                                     4. Shared understanding of metrics
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     The fourth idea is to build more knowledge in the open source ecosystem about how metrics can help us understand the impact and health of open source projects. The Linux Foundation initiated the CHAOSS (Community Health Analytics Open Source Software) project to bring open source projects and other stakeholders together to build a shared understanding of metrics and of the software tools to capture and analyze said metrics. This blog post is based on research conducted as part of the <a href="https://chaoss.community/" target="_blank" rel="noopener">CHAOSS project</a>.
>                                                   </p>
>                                                   
>                                                   <h2>
>                                                     Acknowledgments
>                                                   </h2>
>                                                   
>                                                   <p>
>                                                     This article is based on the whitepaper <a href="https://digitalcommons.unomaha.edu/isqafacpub/62/" target="_blank" rel="noopener">Regression Analysis of Open Source Project Impact: Relationships with Activity and Rewards</a> by Vinod K. Ahuja. Graphics were prepared by Kevin M. Lumbard. This work is supported by Mozilla and the Alfred P. Sloan Foundation.
>                                                   </p></blockquote>
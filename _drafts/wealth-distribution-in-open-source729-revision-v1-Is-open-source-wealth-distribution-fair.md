---
id: 733
title: Is open source wealth distribution fair?
date: 2018-11-29T16:31:41-06:00
author: Georg Link
layout: revision
guid: http://www.georglink.de/2018/11/29/729-revision-v1--733
permalink: /2018/11/29/729-revision-v1--733
---
I published the following blog post [originally on Opensource.com](https://opensource.com/article/18/12/wealth-open-source-distributed).

> <div class="os-article__middle">
>   <div class="panel-pane pane-entity-field pane-node-body">
>     <div class="field field-name-body field-type-text-with-summary field-label-hidden">
>       <div class="field-items">
>         <div class="field-item even">
>           <p>
>             If <a href="https://en.wikipedia.org/wiki/Wealth" target="_blank" rel="noopener">wealth</a> is the abundance of valuable possessions, open source has a wealth of software. While no one “owns” open source, some are better than others at converting this communal wealth to personal wealth.
>           </p>
>           
>           <p>
>             Many open source project maintainers who produce free open source software do not have a model for deriving income from the assets they have created. However, companies that use open source software to enhance their products and services convert this valuable asset into income.
>           </p>
>           
>           <p>
>             The open source ecosystem needs novel mechanisms to distribute privatized wealth back to maintainers if open source projects are to remain sustainable. In this post, I&#8217;ll discuss the challenges of distributing wealth more fairly, starting with three key observations:
>           </p>
>           
>           <ul>
>             <li>
>               We need to identify projects that are important and need funding.
>             </li>
>             <li>
>               We lack fair rules for distributing money among open source project contributors.
>             </li>
>             <li>
>               Transaction costs are too high in underbanked areas. <a href="https://bugmark.net/" target="_blank" rel="noopener">Bugmark</a> and <a href="https://erlend-sh.github.io/ossgrants/" target="_blank" rel="noopener">ossgrants</a> (both discussed below) are two project ideas for addressing this problem.
>             </li>
>           </ul>
>           
>           <h2>
>             Wealth creation in open source
>           </h2>
>           
>           <p>
>             The wealth created by open source rests today on an imbalance between those who bear the costs and those who enjoy the income. Consider the following example:
>           </p>
>           
>           <p>
>             An amateur developer creates an open source project as a side project or hobby and releases the software <a href="https://opensource.org/licenses" target="_blank" rel="noopener">free of charge</a>. The software increases communal wealth when users derive value from it. Companies in particular leverage the open source software in their innovation stream, building products and services with less investment and converting valuable open source software assets into income.
>           </p>
>           
>           <p>
>             A growing user base brings more support inquiries, bug reports, and feature requests, which take more time and increase costs for the maintainer. A community of contributors might form and share the work of developing and maintaining the software. Sharing the cost of creating communal wealth by contributing, however, does not provide income for the maintainer, who cannot generate personal wealth without mechanisms that distribute income from other users.
>           </p>
>           
>           <p>
>             It is important to recognize that maintainers need to make a living, and if they have no income from open source projects, they likely have another job—which reduces the time they can spend on maintaining open source software. A lack of funding for open source projects becomes problematic when the <a href="https://www.fordfoundation.org/about/library/reports-and-studies/roads-and-bridges-the-unseen-labor-behind-our-digital-infrastructure" target="_blank" rel="noopener">software is part of our modern infrastructure and requires long-term maintenance</a>.
>           </p>
>           
>           <div class="media media-element-container media-default media-wysiwyg-align-center">
>             <div id="file-415781" class="file file-image file-image-jpeg">
>               <div class="content">
>                 <p>
>                   <div id="attachment_731" style="width: 559px" class="wp-caption aligncenter">
>                     <a href="http://www.georglink.de/media/2018/11/2018-11-17_model.png"><img aria-describedby="caption-attachment-731" loading="lazy" class="wp-image-731 size-full" src="http://www.georglink.de/media/2018/11/2018-11-17_model.png" alt="The relationship between those who create open software and those who generate income from this communal wealth." width="549" height="345" srcset="http://www.georglink.de/media/2018/11/2018-11-17_model.png 549w, http://www.georglink.de/media/2018/11/2018-11-17_model-300x189.png 300w" sizes="(max-width: 549px) 100vw, 549px" /></a>
>                     
>                     <p id="caption-attachment-731" class="wp-caption-text">
>                       The relationship between those who create open software and those who generate income from this communal wealth.
>                     </p>
>                   </div>
>                 </p>
>                 
>                 <div class="field field-name-field-file-image-caption field-type-text-long field-label-hidden">
>                   <div class="field-items">
>                     <div class="field-item even">
>                       <p class="rtecenter">
>                         </div> </div> </div> </div> </div> </div> 
>                         
>                         <p>
>                           The question then becomes: How can the wealth created by use of open source software be distributed to support long-term maintenance by paying maintainers?
>                         </p>
>                         
>                         <p>
>                           At <a href="https://mozillafestival.org/" target="_blank" rel="noopener">MozFest 2018</a>, 23 people gathered to discuss this question. In small groups, participants discussed problems of interest, chose one problem to work on, and later presented their solutions to the larger group. This post summarizes key takeaways from this presentation and draws on ideas discussed during <a href="https://sustainoss.org/" target="_blank" rel="noopener">Sustain Summit 2018</a>.
>                         </p>
>                         
>                         <div class="media media-element-container media-default media-wysiwyg-align-center">
>                           <div id="file-415786" class="file file-image file-image-png">
>                             <p>
>                               <div id="attachment_730" style="width: 610px" class="wp-caption aligncenter">
>                                 <a href="http://www.georglink.de/media/2018/11/2018-11-17_grouphoto.png"><img aria-describedby="caption-attachment-730" loading="lazy" class="wp-image-730 size-full" src="http://www.georglink.de/media/2018/11/2018-11-17_grouphoto.png" alt="Participants in MozFest 2018 met to discuss open source wealth distribution." width="600" height="275" srcset="http://www.georglink.de/media/2018/11/2018-11-17_grouphoto.png 600w, http://www.georglink.de/media/2018/11/2018-11-17_grouphoto-300x138.png 300w" sizes="(max-width: 600px) 100vw, 600px" /></a>
>                                 
>                                 <p id="caption-attachment-730" class="wp-caption-text">
>                                   Participants in MozFest 2018 met to discuss open source wealth distribution.
>                                 </p>
>                               </div>
>                             </p>
>                             
>                             <p>
>                               &nbsp;
>                             </p>
>                           </div>
>                         </div>
>                         
>                         <h2>
>                           Why and how to share wealth
>                         </h2>
>                         
>                         <p>
>                           A central question is this: Why would companies share the income they generate from using open source software?
>                         </p>
>                         
>                         <p>
>                           For-profit companies are seen as profit maximizers, and sharing revenue with open source maintainers, who license their intellectual property for free, seems counterintuitive. One survey found that 50% of respondents believe that <a href="https://www.digitalocean.com/currents/october-2018/#how-other-companies-are-doing" target="_blank" rel="noopener">large tech companies gain more from using open source than they contribute</a>, which demonstrates that companies generate means to give back by using open source. (Note that I am not referring to the many open source projects companies actively maintain, or those that a company started. The focus here is on volunteer-driven communities.)
>                         </p>
>                         
>                         <p>
>                           Three concrete value propositions can convince a company to pay open source maintainers:
>                         </p>
>                         
>                         <ul>
>                           <li>
>                             Donating to open source projects earns a good name within the open source ecosystem. Donating to a project or a maintainer—for example via <a href="https://www.patreon.com/" target="_blank" rel="noopener">Patreon</a>, <a href="https://opencollective.com/" target="_blank" rel="noopener">OpenCollective</a>, or an open source foundation—funds development work without exerting influence.
>                           </li>
>                           <li>
>                             Funding open source maintenance ensures that an open source project will be updated and vulnerabilities fixed, which is important for companies that rely on the software for their products, services, and infrastructure.
>                           </li>
>                           <li>
>                             A company gains influence over the strategic direction of an open source project when a donation or membership fee is rewarded with access to core maintainers. Special access can require that maintainers sign non-disclosure agreements and help develop solutions for vulnerabilities that may not yet have been publicly disclosed.
>                           </li>
>                         </ul>
>                         
>                         <p>
>                           An open source project can also start a company that provides hosting and support services, and collect funds by selling their services. This is the most formalized way of securing funds and provides a clear value proposition. The key point is that a maintainer must figure out how to participate in the economy around open source software.
>                         </p>
>                         
>                         <h2>
>                           Distributing wealth: 3 practical issues
>                         </h2>
>                         
>                         <p>
>                           The following issues arise when the donation model is used:
>                         </p>
>                         
>                         <p>
>                           First, not every project benefits equally from funds. Do you rely on open source software that might become unsupported if you do not donate to the project? The goal of such an evaluation is to find weak spots in an open source supply chain that can be strengthened with the least amount of cost. Consider using metrics, like the ones created by the <a href="https://chaoss.community/" target="_blank" rel="noopener">CHAOSS project</a>, for determining the health of an open source project. How exactly to identify open source projects that need funding before they become unmaintained is an unsolved problem. The <a href="https://www.coreinfrastructure.org/" target="_blank" rel="noopener">Core Infrastructure Initiative</a> has developed the <a href="https://www.coreinfrastructure.org/programs/census-project/" target="_blank" rel="noopener">Census Project</a> to work on a solution. <a href="https://tidelift.com/" target="_blank" rel="noopener">TideLift</a> takes an innovative approach, paying <a href="https://blog.tidelift.com/1m-to-pay-open-source-maintainers-on-tidelift" target="_blank" rel="noopener">more than $1 million to open source project maintainers</a> based on how much a project is used.
>                         </p>
>                         
>                         <p>
>                           Second, how should funds be distributed among open source project members? Defining how donations will be used should be declared upfront to avoid conflict. One approach might be to recognize individual contributors based on their contributions. For example, you could distribute funds based on the number of issues closed, commits accepted, lines added, wiki pages edited, documentation pages revised, forum messages posted, blog posts published, or other quantifiable contributions. But not all contribution types to a project can be measured—for example, organizing meetings and presenting at conferences are valuable but time-intensive contributions that do not produce trace data in a collaboration software. Every project must set its own rules, but we can share stories and best practices. <a href="https://opencollective.com/" target="_blank" rel="noopener">Open Collective</a> brings this conversation to the public.
>                         </p>
>                         
>                         <p>
>                           Third, transaction costs hinder fair distribution of the wealth created by open source. Specifically, many people in underbanked regions struggle with the logistics of receiving payments. When an open source team member must wait for hours to cash a check, the cost of the time might outweigh the amount they receive for their work. This very real problem may be beyond the scope of what open source projects can do (except perhaps initiatives for <a href="https://web3.foundation/" target="_blank" rel="noopener">Web3</a>), but it deserves attention. Ultimately, the solution is to bring banking to all people and improve the interoperability of banking systems around the world.
>                         </p>
>                         
>                         <h2>
>                           Facilitating and incentivizing wealth transfer
>                         </h2>
>                         
>                         <p>
>                           There are many initiatives to solve the sustainability problem in open source, but I&#8217;ll highlight two projects that I find intriguing.
>                         </p>
>                         
>                         <p>
>                           <a href="https://bugmark.net/" target="_blank" rel="noopener">Bugmark</a> answers the question of who within an open source project should get paid, and how much, by creating a <a href="https://blog.zgp.org/smart-futures-contracts-on-software-issues-talk-and-bullshit-walks/" target="_blank" rel="noopener">marketplace that introduces price signals to open source</a>. The Bugmark exchange allows trading on the status of an issue—for example, issues listed by an open source project on their GitHub issue tracker. <a href="https://blog.zgp.org/some-ways-that-bug-futures-markets-differ-from-open-source-bounties/" target="_blank" rel="noopener">Unlike bug bounties</a>, trading on the status of an issue is <a href="https://blog.zgp.org/are-bug-futures-just-high-tech-piecework/" target="_blank" rel="noopener">independent of doing work</a>. By decoupling payment and work, Bugmark has the potential to fund open source work that is not reliant on fixing an issue. For example, a project member who does bug triaging, an honorable but tedious task, has in-depth knowledge of how a project is doing and what is being worked on. This person can use their insider knowledge to trade on Bugmark and earn money. For more details on how Bugmark works, I recommend this <a href="https://weis2018.econinfosec.org/wp-content/uploads/sites/5/2016/09/WEIS_2018_paper_27.pdf" target="_blank" rel="noopener">publication</a>.
>                         </p>
>                         
>                         <p>
>                           <a href="https://erlend-sh.github.io/ossgrants/" target="_blank" rel="noopener">Funding Index</a> is an early-stage idea that revolves around donations. Donations provide a project with money without restrictions. Donations benefit companies, but the publicity effect is short-lived. At SustainSummit, we developed an idea to capture donations more permanently and create a funding index. Donations would be logged and aggregated across companies and projects. Similar to consumer rating agencies that rate products and services, this index would rate companies by how much they donate to open source projects relative to how many employees they have. We could produce badges for “#1 donor to open source,” “#1 donor to infrastructure open source projects,” or “#1 mid-sized company donor to open source.” Such a badge would extend the publicity effect of donations and hopefully incentivize companies to donate more. <a href="https://erlend-sh.github.io/ossgrants/" target="_blank" rel="noopener">Funding Index</a> exists in a first <a href="https://erlend-sh.github.io/ossgrants/" target="_blank" rel="noopener">prototype</a> and welcomes discussions on the <a href="https://discourse.sustainoss.org/c/corporate-contributions/funding-index" target="_blank" rel="noopener">Discourse Forum</a>.
>                         </p>
>                         
>                         <h2>
>                           Sustainability is more than funding
>                         </h2>
>                         
>                         <p>
>                           Funding helps to pay for living expenses, servers, stickers, and travel to conferences to enable face-to-face collaboration. Funding is a necessary component of a sustainable open source project, but it requires additional elements.
>                         </p>
>                         
>                         <p>
>                           A sustainable open source project fosters a healthy community, which is welcoming, provides a productive work environment, supports its members, and is prepared to let members move on when their focus in life changes. These governance and community concerns build the foundation from which open source projects work, and once they are in place, funding can leverage the work and help project members excel.
>                         </p>
>                         
>                         <p>
>                           A final thought: Companies that are willing to financially support open source projects need to see the business value. Currently, there is no single solution that fits all open source project contexts. Every open source project may need to experiment for themselves and find a way to secure funds. <a href="https://umbraco.com/" target="_blank" rel="noopener">Umbraco</a>, for example, built a <a href="https://umbraco.com/blog/profit-through-generosity/" target="_blank" rel="noopener">sustainable business</a> around its open source CMS system and has experimented with 11 different business models since its inception in 2004.
>                         </p>
>                         
>                         <p>
>                           More conversations are needed, and experiences must be shared. <a href="https://sustainoss.org/about/" target="_blank" rel="noopener">SustainOSS.org</a> brings sustainers together to have these <a href="https://discourse.sustainoss.org/" target="_blank" rel="noopener">conversations</a>. In conclusion, fair distribution of the wealth created by open source can enhance what already works well in open source, but it will not replace traditional open source practices.
>                         </p>
>                         
>                         <h2>
>                           Post Scriptum
>                         </h2>
>                         
>                         <p>
>                           I acknowledge that companies and foundations also create open source projects. Sustainability issues exist nonetheless, and takeaways transfer.
>                         </p>
>                         
>                         <h2>
>                           Acknowledgments
>                         </h2>
>                         
>                         <p>
>                           I&#8217;d like to thank all MozFest 2018 session participants, especially the note-takers. I appreciate constructive feedback from Sean Goggins and Tobie Langel. I received a <a href="https://events.linuxfoundation.org/travel-fund-request/" target="_blank" rel="noopener">Linux Foundation Community Travel Fund</a> to present at Open Source Summit Europe 2018 in Edinburgh, which allowed me to participate in the SustainSummit and MozFest in London later during the same week. This work is supported through the Alfred P. Sloan Foundation Digital Technology grant on Open Source Health and Sustainability, Num: <a href="https://sloan.org/grant-detail/8434" target="_blank" rel="noopener">8434</a>
>                         </p></div> </div> </div> </div> </div> 
>                         
>                         <p>
>                           &nbsp;
>                         </p></blockquote>
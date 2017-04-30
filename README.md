# web-tool-riskcalculator

 <img src="images/risk-calculator.png" height="600px" width="auto">
 
<h2>Background</h2>
<p>
At my previous company, I was the subject matter expert for a specific sales contract exhibit involving a performance guarantee. This guarantee was technical in nature and based off of an international IEC standard. As a result, negotiations of this exhibit with customers was often complicated and typically involved some deviations from both the IEC standard and from our company's internal guidelines. These deviations often added to an already difficult-to-quantify risk of failing the performance guarantee, with associated liquidated damages in the millions of dollars.
</p>
<p>
Due to the risk involved, the approval process for any contract deviations was managed by a team of performance specialists. As the number of contracts (and requested deviations) increased globally, this approval process increasingly became a bottle-neck in terms of turn-around time and put pressure on the contract signing schedule. A team of local subject matter experts, local sales contractor negotiators, and the performance specialists worked together to develop a process that codified typical deviations and their associated risk impacts in order to streamline the approval process. 
</p>
<p>
I worked closely with the chief performance specialist to turn these risk calculation methodologies into a web-based tool, the Risk Calculator. This tool was eventually used by teams around the globe and (i) allowed local contract negotiation teams to better assess deviations to the performance guarantee, (ii) improve communications with the performance specialists during the deviation approval process, and (iii) decrease turn-around time of the approval process by off-loading the risk calculations from the performance specialists. 
</p>
<p>
Unfortunately, no source code of the final web-based Risk Calculator is included due to IP concerns. However, this documentation is meant to highlight the thought-process behind the problem (contract deviations) and the solution (a risk calculator)... 
<ul>
<li>Performance Guarantee - what was being negotiated</li>
<li>Deviations and Risk - why a process and tool was needed
<li>Risk Calculator - how it works
</ul>
</p>
<h2>Performance Guarantee</h2>
<p>
The performance guarantee stated that a product under test would meet or exceed a specified threshold within a margin of uncertainty. An IEC standard was used to test the product, which specified everything from test equipment to performance calculations to methods of estimating test uncertainty. Additionally, the company had internal guidelines above and beyond the IEC standard to specify certain aspects of the test.
</p>
<p>
Depending on real world constraints, customers would often request deviations from either the IEC standard or the company guidelines. The default contract exhibit had a standard level of risk associated with passing or failing the performance guarantee, based on historical performance test results. Failing a test could potentially involve a substantial amount of money in the form of liquidated damages, therefore estimating the risk of failure was an important part of the contract approval process. 
</p>
<h2>Deviations and Risk</h2>
<p>
When a contract was being negotiated, any requested deviations to the baseline performance guarantee had to be approved by a team of performance specialists. This typically involved estimating the impact of each individual deviation, and estimating an overall risk of failure accounting for all of the requested deviations.  
</p>
<p>
I worked closely with the team of performance specialists to identify a list of deviations that were commonly requested during contract negotiations. For each of these deviations, we developed the rules by which they impacted the overall risk estimate. I was then responsible for implementing these rules and additional inputs into a web-based tool, the Risk Calculator.
</p>

<h2>Risk Calculator</h2>
<img src="images/risk-calculator.png" height="600px" width="auto">
<p>
The Risk Calculator consisted of four main components: Inputs, Deviations, Outputs and Contact Info.
</p>







 
 
 <img src="images/normal-distribution.png" height="400px" width="auto">
 

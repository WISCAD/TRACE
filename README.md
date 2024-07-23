# TRACE
TRACE: Fast and Accurate Trace Signal Selection for Post-Silicon Debug of ICs

Supported by **NSF CAREER award 1053496**

**Related Publications:** 

M. Li, and A. Davoodi, "A hybrid approach for fast and accurate trace signal selection for post-silicon debug", IEEE Trans. on CAD (TCAD'14), Vol. 33, No. 7, pp. 1081 - 1094, June 2014; also in Design, Automation, and Test in Europe (DATE'13), pp. 485-490, March 2013; and in Int'l Workshop on Microprocessor Test and Verification (MTV'12), December 2012. (Slides)

M. Li, and A. Davoodi, "Multi-mode trace signal selection for post-silicon debug", Asia and South Pacific Design Automation Conf. (ASPDAC'14), pp. 640-645, January 2014. (Slides)

This repo provides binary and benchmarks and documentation.

Please read the included README_detailed.txt file; it has information about how runtime should be correctly measured.

Also included is the set of original benchmarks to be used with the binary. The README file explains about setting the control signals for the relevant benchmarks. It's crucial to correctly use them for fair comparison among approaches.

The TRACE binary only generates a trace signal solution. It does not report its quality in terms of the State Restoration Ratio metric. Please make it clear in any publication for fair comparison if, (1) same evaluator has been used to evaluate solutions from different approaches, (2) clarify that there is a distinction between a binary generating a solution and an evalutor tool measuring its quality.

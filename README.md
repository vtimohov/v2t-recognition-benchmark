# v2t-recognition-benchmark

EXPERIMENT EXPLANATION

CONTEXT: We utilize a third-party service for voice-to-text transcription. The output of this process yields a set of texts. Subsequently, we employ these texts as context for our Question Answering solution. Therefore, it is imperative to ensure that the voice-to-text (V2T) service provides satisfactory text quality.

GOAL: a benchmark enabling the estimation of text quality.

HOW TO: Let us assume that satisfactory text content consists solely of English words, along with some names, toponyms, etc. So we can use next equation: 
$$
\begin{equation*}
s=\ \frac{t_{b}}{t_{g}} \ *\ 100\%
\end{equation*}
$$
Where $t_{g}$ is a total number of words is a text dictinary. And $t_{m}$ is bad tokens in this dictinary.

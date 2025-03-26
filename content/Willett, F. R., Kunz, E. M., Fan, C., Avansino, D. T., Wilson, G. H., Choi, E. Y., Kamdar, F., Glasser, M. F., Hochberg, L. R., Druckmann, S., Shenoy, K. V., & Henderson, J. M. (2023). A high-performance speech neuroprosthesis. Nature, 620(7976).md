# Willett, F. R., Kunz, E. M., Fan, C., Avansino, D. T., Wilson, G. H., Choi, E. Y., Kamdar, F., Glasser, M. F., Hochberg, L. R., Druckmann, S., Shenoy, K. V., & Henderson, J. M. (2023). A high-performance speech neuroprosthesis. Nature, 620(7976), 1031–1036

<https://doi.org/10.1038/s41586-023-06377-x>

Intracortical BCI using microelectrode array, attempted and internal speech. Achieved 9.1% WER on a 50 word vocabulary and 23.8% WER on 125k word vocabulary (“first successful demonstration of large-vocabulary decoding”). Decoded speech at 62 WPM. All these figures are integer-factor improvements over previous SotA.

Pretty simple model, at a high level: threshold crossings are decoded by RNN into phonemes; then onward into Kaldi as usual for ASR.

Same first and senior authors as the very impressive earlier:

> High-performance brain-to-text communication via handwriting. Francis R. > Willett, Donald T. Avansino, Leigh R. Hochberg, Jaimie M. Henderson & > Krishna V. Shenoy. <https://www.nature.com/articles/s41586-021-03506-2>)

# Machine Translation using Attention mechanism

Machine translation was traditionally done via *encoder-decoder* blocks, where the former receives the sequence of data, outputs a context, which will form the input of the decoder network. So the entire input should first pass the encoder, and then the decoder starts to output predicted words one by one. However, this is not the usual way that humans translate. Given a German paragraph, we usually translate part by part, where we need to attend to most relevant parts. This inspires attention mechanism, in which we assign weights (learnable parameters) to each input. Then, based on the activations and attentions, we have a context feeding in for the prediction purpose.

In this notebook, we implement a neural machine translation using the attention mechanism.

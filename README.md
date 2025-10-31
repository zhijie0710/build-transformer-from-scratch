# build-transformer-from-scratch
Practice building a transformer from scratch with python

Fundamental blocks of a transformer:   
 a.) Encoder
 b.) Decoder

Components of encoder/decoder blocks:   
 a.) one Encoder block
   1. embedding inputs
   2. positional encoding
   3. MHA: multi-head attention (layer norm + Residual connection)
   4. FFN: feed-forward network (layer norm + Residual connection)  
 b.) one Decoder block
   1. embedding inputs
   2. positional encoding
   3. MHA: multi-head attention (layer norm + Residual connection)
   4. Cross-attention (layer norm + Residual connection)
   5. FFN: feed-forward network (layer norm + Residual connection)

* (layer norm + Residual connection) is implemented using pre-LN:  x+Sublayer(LayerNorm(x))

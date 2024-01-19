# CausalAdv:Adversarial Robustness through the lens of causality
Link to the Paper: [Arxiv](https://arxiv.org/pdf/2106.06196.pdf)

Deep Neural Networks, though seemingly accurate, can be easily fooled by small, intentional changes in the input data called adversarial attacks.This highlights the need for robust models that maintain accuracy even under such attacks. Thus, the paper attempts to train the model on such adversarial examples in order to become resistant/robust against such manipulations in the data.

*Prerequisites*
-------------
- `Python 3.10`
- GPU
- Install necessary packages using `pip install -r requirements.txt`
----------
- Run the Following command:
```bash
python causaladv_utils.py
```
and
```bash
python causaladv.py
```
- Initially, comment out lines 214-250 in `causaladv.py`, and uncomment line 213 (run the model from scratch) to obtain `cifar10-adam_13-best.pth`.
- After model is trained, comment out line 213 and uncomment lines 214-250 to check model robustness.
- In case of a CPU machine, run on Google Colab with runtime type: T4 GPU

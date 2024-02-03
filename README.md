#  Generative Input
Here is the datasets accompanying the paper [Generative Input: Towards Next-Generation Input Methods Paradigm.](https://browse.arxiv.org/abs/2311.01166)
* __XF-Datasets__: We built this dataset to evaluate three typical tasks in input methods. Here, we provide the full test set and part of the training set.
    * we constructed test sets for IntelAssoc and ConvAssist with 2K samples each for manual evaluation. For the evaluation of FK2C effects under different keyboards of 26-key and 9-key, we constructed a test set of 57K, covering different input modes such as perfect pinyin, abbreviated pinyin, random abbreviated pinyin, and noisy input with different error types. 
* __PDTP__: PD dataset and TP dataset are publicly available datasets commonly used to evaluate the P2C effect of input methods. We obtain this test set from [OpenIME](https://github.com/cooelf/OpenIME?tab=readme-ov-file) and fix part of the phonetic notation issues

##  Tasks and data examples    
  An example of each subtask is as follows.
  | Task  | Task Description | Input  | Output  |
  | :----- | :----- | :------ | :------ |
  | IntelAssoc | 根据用户已输入的句子，续写可能的下一句。(Based on the sentence the user has already entered, write the next possible sentence.) | 用户输入：我今天没时间 (User input: I don't have time today) | 明天可以吗 (How about tomorrow) |
  | ConvAssist | 将用户输入的句子，改写成更加精彩的句子。(Rewrite the user's input into something better.)                                                                                                          | 用户输入：秋天来了 (User input: Autumn is coming)   | 🍂秋天到了，缤纷的树叶掉落一地，让我们一起享受这美好的季节吧！(🍂Autumn is coming, colorful leaves fall down, let's enjoy this beautiful season!) |
  | FK2C  | 在输入法中，根据用户输入的按键序列，解码出合理的拼音切分与对应的中文结果。(Please decode the reasonable pinyin segmentation and corresponding Chinese characters according to the key sequence entered by the user) | 用户输入：woaiini (User input: woaiini) | Wo'Aii'Ni，我爱你 (Wo'Aii'Ni, I love you) |

##  Code and model
  We are based on the [iFlytekSpark](https://gitee.com/iflytekopensource) for development, the relevant code and model have been open source.

##  Reference
  If you use this repo please cite our paper:
  >   @misc{ding2023generative,
      title={Generative Input: Towards Next-Generation Input Methods Paradigm}, 
      author={Keyu Ding and Yongcan Wang and Zihang Xu and Zhenzhen Jia and Shijin Wang and Cong Liu and Enhong Chen},
      year={2023},
      eprint={2311.01166},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}

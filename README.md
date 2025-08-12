# LLM-colab-pipeline

A comprehensive pipeline for Large Language Model development with Google Colab notebooks, including inference optimization and reinforcement learning training methods.

## 🚀 Features

- **T4-Safe Inference**: Optimized for Google Colab T4 GPUs with memory-efficient mixed precision
- **Multiple RL Training Methods**: PPO, DPO, and ORPO implementations
- **Ready-to-Use Notebooks**: Pre-configured Colab notebooks for immediate deployment
- **Production-Ready Code**: Error handling, memory optimization, and best practices

## 📁 Project Structure

```
LLM-colab-pipeline/
├── requirements.txt              # Python dependencies
├── nb/                          # Notebook directory
│   ├── GPT_OSS_MXFP4_(20B)-Inference-T4-safe.ipynb  # GPT inference notebook
│   └── RL/                      # Reinforcement Learning notebooks
│       ├── PPO_colab_demo.ipynb    # Proximal Policy Optimization
│       ├── DPO_colab_demo.ipynb    # Direct Preference Optimization
│       └── ORPO_colab_demo.ipynb   # Odds Ratio Preference Optimization
└── README.md                    # This file
```

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/procop07/LLM-colab-pipeline.git
   cd LLM-colab-pipeline
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## 📚 Notebooks Guide

### 🔥 Inference Notebook

**[GPT_OSS_MXFP4_(20B)-Inference-T4-safe.ipynb](./nb/GPT_OSS_MXFP4_(20B)-Inference-T4-safe.ipynb)**

- **Purpose**: T4-safe inference for large language models (up to 20B parameters)
- **Features**: 
  - Mixed precision (FP4) quantization
  - Memory-efficient loading
  - Error handling and safe inference
- **Compatible with**: T4, P100, V100 GPUs

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/procop07/LLM-colab-pipeline/blob/main/nb/GPT_OSS_MXFP4_(20B)-Inference-T4-safe.ipynb)

### 🎯 Reinforcement Learning Notebooks

#### **[PPO_colab_demo.ipynb](./nb/RL/PPO_colab_demo.ipynb)**

- **Algorithm**: Proximal Policy Optimization
- **Use Case**: RLHF (Reinforcement Learning from Human Feedback)
- **Features**: Reward model integration, policy optimization

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/procop07/LLM-colab-pipeline/blob/main/nb/RL/PPO_colab_demo.ipynb)

#### **[DPO_colab_demo.ipynb](./nb/RL/DPO_colab_demo.ipynb)**

- **Algorithm**: Direct Preference Optimization
- **Use Case**: Simpler alternative to RLHF without reward model
- **Features**: Preference-based training, stable optimization

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/procop07/LLM-colab-pipeline/blob/main/nb/RL/DPO_colab_demo.ipynb)

#### **[ORPO_colab_demo.ipynb](./nb/RL/ORPO_colab_demo.ipynb)**

- **Algorithm**: Odds Ratio Preference Optimization
- **Use Case**: Reference-model-free alignment
- **Features**: Memory efficient, single-stage training

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/procop07/LLM-colab-pipeline/blob/main/nb/RL/ORPO_colab_demo.ipynb)

## 🚦 Quick Start

### For Inference:
1. Open the [GPT Inference notebook](./nb/GPT_OSS_MXFP4_(20B)-Inference-T4-safe.ipynb) in Colab
2. Run all cells to install dependencies
3. Replace the model name with your desired model
4. Execute the inference pipeline

### For RL Training:
1. Choose your preferred RL method (PPO, DPO, or ORPO)
2. Open the corresponding notebook in Colab
3. Prepare your training data in the specified format
4. Run the training pipeline

## 💡 Usage Tips

- **GPU Requirements**: T4 or higher recommended for inference, P100+ for training
- **Memory Management**: Use gradient checkpointing for large models
- **Batch Sizes**: Start small (1-2) and increase based on available memory
- **Monitoring**: Use wandb integration for experiment tracking

## 🔧 Customization

### Adding New Models
1. Update the model name in the notebook configuration
2. Adjust quantization settings if needed
3. Modify generation parameters as required

### Custom Training Data
1. Follow the data format shown in the notebooks
2. Ensure proper prompt-response structure
3. Balance positive and negative examples

## 📈 Performance

| Model Size | Method | T4 GPU | Training Time | Memory Usage |
|------------|--------|---------|---------------|-------------|
| 7B         | DPO    | ✅      | ~2 hours      | ~14GB       |
| 13B        | PPO    | ⚠️      | ~4 hours      | ~15GB       |
| 20B        | ORPO   | ❌      | N/A           | >16GB       |

**Legend**: ✅ Recommended, ⚠️ Possible with optimizations, ❌ Not recommended

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Links

- **Repository**: [https://github.com/procop07/LLM-colab-pipeline](https://github.com/procop07/LLM-colab-pipeline)
- **Issues**: [Report bugs and request features](https://github.com/procop07/LLM-colab-pipeline/issues)
- **Discussions**: [Community discussions](https://github.com/procop07/LLM-colab-pipeline/discussions)

## ⭐ Star History

If you find this project helpful, please consider giving it a star! ⭐

---

**Made with ❤️ for the LLM community**

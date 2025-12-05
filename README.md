# Adversarial-robustness-is-critical-for-safe-AI-deployment
adversarial robustness comparing ResNet-18 and Vision Transformer models on CIFAR-10. Using FGSM and PGD attacks at multiple perturbation levels (ε ∈ {2, 4, 8, 16}/255), 
 I demonstrated that ResNet-18 maintains 21.1% accuracy under strong PGD attacks at ε=8/255, while Vision Transformer accuracy drops to 1.8%, revealing critical architecture-dependent robustness trade-offs. 
 This research has been documented in a peer-reviewed paper with fully reproducible code, demonstrating my ability to design experiments independently. 
 implement adversarial methods, analyse results, and communicate findings at publication quality."

text
# Adversarial Robustness: CNN vs Vision Transformer

Evaluating the robustness of ResNet-18 and Vision Transformer (ViT-Tiny) 
against FGSM and PGD adversarial attacks on CIFAR-10.

## Key Findings

- **ResNet-18 Clean Accuracy**: 84.9%
- **ViT-Tiny Clean Accuracy**: 73.8%
- **ResNet-18 is more robust**: At ε=8/255 under PGD, ResNet retains 21.1% 
  accuracy while ViT drops to 1.8%

## Results Summary

| ε (×/255) | ResNet FGSM | ResNet PGD | ViT FGSM | ViT PGD |
|-----------|-------------|-----------|---------|---------|
| 2         | 46.04%      | 41.14%    | 28.43%  | 14.23%  |
| 4         | 43.41%      | 32.74%    | 25.36%  | 6.18%   |
| 8         | 38.00%      | 21.11%    | 20.36%  | 1.78%   |
| 16        | 29.12%      | 14.54%    | 14.25%  | 0.77%   |

## How to Run

### On Google Colab
1. Open: `Adversarial_robustness_is_critical_for_safe_AI_deployment.ipynb`
2. Paste into Google Colab
3. Run all cells (requires GPU, ~1-2 hours)

### Requirements
- PyTorch
- torchvision
- timm
- pandas
- matplotlib

Install with:
pip install torch torchvision timm pandas matplotlib

text

## Files

- `Adversarial_robustness_is_critical_for_safe_AI_deployment.ipynb` - Full notebook with training + attacks
- `adversarial_robustness_is_critical_for_safe_ai_deployment.py` - Standalone Python script
- `results.csv` - Experimental results table
- `robustness_curves.png` - Robustness plots (FGSM vs PGD)

## Research Paper

Full peer-review ready paper: `research_paper.pdf` (5 pages)

## Citation

If you use this code, please cite:

@misc{adversarial_robustness_2025,
title={Evaluating the Robustness of CNN and Vision Transformer Models
Against Adversarial Attacks Using FGSM and PGD},
author={Your Name},
year={2025},
howpublished={\url{https://github.com/shri33/Adversarial-robustness-is-critical-for-safe-AI-deployment}}
}

text

## License

MIT License - See LICENSE file for details
Priority 3: Prepare Erasmus Application Materials (1 hour)
Create a Statement of Purpose / SOP for Erasmus (copy-paste ready):

ERASMUS MUNDUS APPLICATION STATEMENT

"During my preparation for this Master's program, I conducted independent research on adversarial robustness comparing two fundamental vision architectures on CIFAR-10. I implemented and trained ResNet-18 (CNN) and Vision Transformer (ViT-Tiny), then systematically evaluated their vulnerability to FGSM and PGD adversarial attacks across four perturbation budgets (ε ∈ {2, 4, 8, 16}/255).

Key Findings:

ResNet-18 achieved 84.9% clean accuracy; ViT-Tiny achieved 73.8%

ResNet-18 is substantially more robust: at ε=8/255 under PGD, it retains 21.1% accuracy while ViT drops to 1.8%

PGD (iterative) is consistently stronger than FGSM (single-step) attacks

This research demonstrates my ability to independently design experiments, implement state-of-the-art attack methods, conduct rigorous analysis, and communicate findings in publication-ready format. The work has been documented as a 5-page peer-review ready paper and released on GitHub with fully reproducible code (Colab notebook + Python script).

This experience has solidified my commitment to trustworthy AI and adversarial robustness research, which aligns perfectly with the Erasmus Mundus AI Master's program's emphasis on responsible AI development."

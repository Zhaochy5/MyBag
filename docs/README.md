# Quadrotor recurrent spiking disturbance compensation

Simulation data, trained model checkpoints and source code for **Recurrent Spiking Disturbance Compensation for Quadrotor Attitude Control**.

[中文使用说明](README_zh.md)

## Download

Use the **ZIP attachment in [Releases](https://github.com/Zhaochy5/MyBag/releases)** for the complete package. GitHub's automatically generated “Source code” ZIP contains only these repository index files.

The release includes 24 complete training/development episodes, the selected and final trained checkpoints, the complete 211000-update training history, and all 90 saved controller runs from 30 paired tasks. It also contains the simulator/controller sources, six result tables, six figures and a saved-data verification program.

Extract the ZIP, open a terminal in `ras_reproducibility`, and run:

```text
python verify_reproducibility.py --hashes-only
python verify_reproducibility.py
```

Hash-only checking uses Python's standard library. The full saved-data check additionally requires NumPy. These commands check recorded data without new training or controller simulation. The package README describes the separate entry point for new controller reruns and its dependencies.

## Scope

The SNN supplies the disturbance-compensation signal in the control-used z3 channel. The ESO angle/rate feedback and internal updates remain active. The reported repetitions use one fixed trained model, with matched trajectory references and disturbance realizations. All runs, error measures and motor-command records are retained. No special-chip speed or energy result is claimed by this package.

Computer-specific paths are removed in the publication copy. The package records the relation between original and public file identities; numerical arrays, model tensor storage and experimental conditions are preserved. No additional reuse license is specified for this release.

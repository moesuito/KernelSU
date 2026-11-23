# KernelSU — S23 Ultra PR #9 validation fork

> [!IMPORTANT]
> **This fork is a one-off validation build and is not maintained.**
>
> It exists only to build and test [PR #9](https://github.com/diabl0w/KernelSU/pull/9)
> from [diabl0w/KernelSU](https://github.com/diabl0w/KernelSU) on a Samsung Galaxy S23 Ultra
> (SM-S918B, KMI `android13-5.15`).
>
> The prebuilt APK is in the [release](https://github.com/moesuito/KernelSU/releases/tag/samsung-v2.2-pr9-s23-lf).
> Source for the release: branch [`s23-pr9-lf`](https://github.com/moesuito/KernelSU/tree/s23-pr9-lf)
> (`main` @ `76a088c5` + PR #9 `5eed7735` + `.gitattributes` LF fix `70ea01b0`).
>
> **Tested on SM-S918B**, One UI 9 / Android 17, kernel `5.15.197-android13-8`,
> firmware `S918BXXUAGZIF`, with DFRoot temporary root:
>
> - DFRoot `LAUNCH ROOT` succeeds;
> - KernelSU loads the SuperUser list (no infinite "Refreshing…");
> - `adb shell su -c id` returns `uid=0(root)`;
> - module ZIP installation works.
>
> **This fork will not receive updates, security fixes or new device support.**
> Use the upstream project: https://github.com/diabl0w/KernelSU
>
> Do not use the APK on other devices/KMIs. Only `android13-5.15` was validated.
> The APK is signed with a local key; there is no promise of future in-place updates.
>
> Upstream documentation: [docs/README.md](docs/README.md).

---

## Português

Este fork existe apenas para disponibilizar uma build testada do
[PR #9](https://github.com/diabl0w/KernelSU/pull/9) no Galaxy S23 Ultra (SM-S918B,
One UI 9 / Android 17, kernel 5.15.197, KMI `android13-5.15`) com root temporário via DFRoot.

- APK testado: [release samsung-v2.2-pr9-s23-lf](https://github.com/moesuito/KernelSU/releases/tag/samsung-v2.2-pr9-s23-lf)
- Fonte: branch [`s23-pr9-lf`](https://github.com/moesuito/KernelSU/tree/s23-pr9-lf)
- Validado: aba SuperUsuário carrega, `su -c id` retorna `uid=0(root)` e a instalação de módulos funciona.

**Este fork está congelado e não será mantido.** Use o repositório original
[diabl0w/KernelSU](https://github.com/diabl0w/KernelSU). O objetivo era apenas validar o PR #9
enquanto ele não é mergeado. Não use em outros aparelhos/KMIs; só `android13-5.15` foi testado.

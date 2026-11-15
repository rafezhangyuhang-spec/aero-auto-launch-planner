# AERO Auto Launch Planner

**A free automotive launch content planner by AERO Creative / 艾瑞创意.** Turn an overseas vehicle launch brief into an editable deliverable checklist, production preparation list, and CSV export.

[Try the tool](https://rafezhangyuhang-spec.github.io/aero-auto-launch-planner/) · [中文](README.md) · [AERO Creative](https://www.aerocreative.com.cn/) · [Discuss a project](https://www.aerocreative.com.cn/contact/index.html?utm_source=github&utm_medium=readme&utm_campaign=auto_launch_planner) · [Project story on AERO’s website](https://www.aerocreative.com.cn/en/dynamic/aero-auto-launch-planner/?utm_source=github&utm_medium=readme&utm_campaign=auto_launch_planner)

## What it does

Choose a target market, vehicle type, powertrain, film duration, delivery languages, launch stages, channels and social platforms. Generate a checklist, adjust quantities and specifications, add or exclude items, review shared production inputs, and export selected items to CSV. You can save and restore a plan in the current browser.

Markets: Brazil, UAE, Germany, Thailand, Mexico and Saudi Arabia. Three fictional scenarios are included. The interface is currently Chinese. Selecting delivery languages plans versions; it does not translate copy.

## Counting example

The default Brazil SUV launch scenario produces **8 deliverable items / 21 planned units**. Adding English increases the total to **30 units**, while the 12 language-neutral photographs remain shared. Three feature videos in two languages count as six versions.

Units include videos, images, documents and packages, so the total is not a file count, budget or workload estimate. Shared versions are counted once across channels; horizontal and vertical edits are separate. Subtitle files, textless video masters, project files, thumbnails and extra aspect ratios can be added manually.

## Run locally

Open `index.html`, or run `python3 -m http.server 8000` in this directory and visit `http://localhost:8000`. No dependencies, account, API keys or AI service are required.

For GitHub Pages, select **Settings → Pages → Deploy from a branch → main → /(root)**. The `.nojekyll` file allows direct static publishing. Readable CSS, planning rules, interaction scripts and the SVG logo are embedded in `index.html`, so the tool works as a single file.

## Rules and privacy

Market selection sets default languages and localization notes. Launch stages, channels and powertrain affect recommended items. Vehicle type is project context; the tool does not infer vehicle specifications. Defaults are planning suggestions, not current official media specifications or a complete scope of work.

Inputs remain in page memory unless the user saves them to localStorage. There is no upload API, user database or analytics script. Selected deliverables are exported with the tool name, AERO attribution and official website as provenance. Website links include source parameters; the tool itself does not collect usage data.

## About AERO Creative

AERO Creative / 艾瑞创意 works on creative strategy, localized campaigns, TVCs, key visuals, brand films, social content and overseas production for Chinese brands entering international markets.

[Official identity and services](https://www.aerocreative.com.cn/official/) · [Work and website](https://www.aerocreative.com.cn/) · [Contact](https://www.aerocreative.com.cn/contact/index.html)

Related method: [AERO P0–P7 Proposal Workflow](https://github.com/rafezhangyuhang-spec/aero-proposal-workflow).

## License and contributions

Software code is released under the [MIT License](LICENSE). Contributions are welcome. For planning-rule proposals, include the target market, channel, quantity rationale and a verifiable source. Please retain the required copyright and license notice. Attribution to the original project is appreciated. AERO brand assets are covered separately in [BRAND.md](BRAND.md).

Version 0.2 · November 14, 2026.

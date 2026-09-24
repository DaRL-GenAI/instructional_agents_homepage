# Instructional Agents

This is the repository that contains source code for the [website of Instructional Agents](https://darl-genai.github.io/instructional_agents_homepage/).

If you find this useful for your work please cite:
```
@misc{yao2025instructionalagentsllmagents,
  title={Instructional Agents: Reducing Teaching Faculty Workload through Multi-Agent Instructional Design},
  author={Yao, Huaiyuan and Xu, Wanpeng and Turnau, Justin and Kellam, Nadia and Wei, Hua},
  year={2025},
  eprint={2508.19611},
  archivePrefix={arXiv},
  primaryClass={cs.AI},
  url={https://arxiv.org/abs/2508.19611},
}
```

# Website License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

# Studio (browser edition)

`studio/` is a static, framework-free web app served from this site at
<https://darl-genai.github.io/instructional_agents_homepage/studio/>. It runs the Instructional
Agents ADDIE pipeline entirely in the visitor's browser with their own OpenAI-compatible API key
(the key never leaves the browser except to the configured API endpoint).

Files: `studio/index.html`, `studio/studio.css`, `studio/js/` (`llm.js` API client, `prompts.js`
agent prompts mirrored from `instructional_agents/src/ADDIE.py`, `pipeline.js` stage runners,
`slides.js` HTML/Beamer/PPTX rendering, `video.js` TTS + MediaRecorder video, `export.js` ZIP,
`state.js` persistence and audit log, `app.js` UI). No build step: edit and push.

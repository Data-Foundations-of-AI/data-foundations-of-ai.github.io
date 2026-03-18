---
layout: default
title: Seminar Series
permalink: /seminar-series/
---
 
<div class="seminar-page">
  <h1>Seminar Series</h1>
  <p>A bi-weekly public seminar on the Data Foundations of AI.</p>

  <div class="seminar-info-grid">
    <div class="info-card">
      <h3>📅 Format</h3>
      <ul>
        <li>45 minutes: invited talk</li>
        <li>15 minutes: Q&A</li>
      </ul>
    </div>
<!--     <div class="info-card">
      <h3>🕐 Default Time</h3>
      <p>Tuesday 6 PM UTC</p>
    </div> -->
    <div class="info-card">
      <h3>🎙️ Nominate a Speaker</h3>
      <p><a href="https://forms.gle/DV92KecS9RsQGFj96" class="text-link">Submit nomination form</a></p>
    </div>
  </div>

  <p>Click <a href="https://calendar.google.com/calendar/u/1?cid=Y180MzA4NmNkYTAyZTZkYjEyNDZiNTU0ZWNkYjhiODE3ZTZmODQ0YmRhNjRiNzI1ZmJkNjRkOTgxMTU3ZWY2N2FlQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20" class="text-link">this link</a> to add the seminar calendar to your Google Calendar.</p>
  <p>Join our <a href="https://groups.google.com/g/dfai-announcement" class="text-link">mailing list</a> for latest announcements (click the "Join group" button in Google Groups).</p>

  <h2 class="section-title">📅 Upcoming Seminars</h2>
  <div class="seminar-calendar">
    <table class="seminar-table">
      <thead>
        <tr>
          <th>Time</th>
          <th>Speaker</th>
          <th>Topic</th>
          <th>Host</th>
          <th>Link</th>
        </tr>
      </thead>
      <tbody>
        <tr class="expandable-row" onclick="toggleDetails('seminar-3')">
          <td>6 PM UTC | 2 PM ET<br>Mar 24, 2026</td>
          <td><a href="https://mayeechen.github.io/" onclick="event.stopPropagation()">Mayee Chen</a></td>
          <td>Olmix: A Framework for Data Mixing Throughout LM Development <span class="expand-indicator">▼</span></td>
          <td>Ishika</td>
          <td onclick="event.stopPropagation()">
            <a href="https://illinois.zoom.us/j/81795451508?pwd=U3PAfk44ZtDJ2BaDJds2FXe2ACsvjg.1" target="_blank" class="text-link">
              Zoom Link
            </a>
          </td>
        </tr>
        <tr class="details-row" id="seminar-3" style="display: none;">
          <td colspan="5">
            <div class="seminar-details">
              <div class="speaker-photo">
                <img src="{{ '/assets/images/seminars/mayee_profile.jpg' | relative_url }}" alt="Mayee Chen">
              </div>
              <div class="seminar-content">
                <h3>Olmix: A Framework for Data Mixing Throughout LM Development</h3>
                
                <h4>Abstract</h4>
                <p>Data mixing---determining the ratios of data from different domains---is a first-order concern for training language models (LMs). While existing mixing methods show promise, they fall short when applied during real-world LM development. We present Olmix, a framework that addresses two such challenges. First, the configuration space for developing a mixing method is not well understood---design choices across existing methods lack justification or consensus and overlook practical issues like data constraints. We conduct a comprehensive empirical study of this space, identifying which design choices lead to a strong mixing method. Second, in practice, the domain set evolves throughout LM development as datasets are added, removed, partitioned, and revised---a problem setting largely unaddressed by existing works, which assume fixed domains. We study how to efficiently recompute the mixture after the domain set is updated, leveraging information from past mixtures. We introduce mixture reuse, a mechanism that reuses existing ratios and recomputes ratios only for domains affected by the update. Over a sequence of five domain-set updates mirroring real-world LM development, mixture reuse matches the performance of fully recomputing the mix after each update with 74% less compute and improves over training without mixing by 11.6% on downstream tasks.</p>
                
                <h4>Bio</h4>
                <p>Mayee Chen is a final-year PhD student in Computer Science at Stanford University, advised by Professor Christopher Ré. Her research focuses on advancing the fundamentals of artificial intelligence through data-centric approaches, particularly in training data curation via techniques she has developed in data mixing, curriculum learning, and weak supervision. Her work has been recognized with a best student paper runner up award at UAI 2022, a best paper award at an AAAI 2022 workshop, and spotlights at ICLR and NeurIPS 2023. Mayee recently was a research intern at the Allen Institute for AI (AI2), driving the data mixing efforts for Olmo 3, their latest open-source large language model. She has also interned at Microsoft Research and obtained her B.S.E. in Operations Research and Financial Engineering from Princeton University.</p>
              </div>
            </div>
          </td>
        </tr>
        <tr>
          <td>Apr 7, 2026</td>
          <td><a href="https://lumos23.github.io/">Luxi He</a></td>
          <td>Data in LLM Lifecycles</td>
          <td>Junwei</td>
          <td onclick="event.stopPropagation()">
            <a href="https://illinois.zoom.us/j/81795451508?pwd=U3PAfk44ZtDJ2BaDJds2FXe2ACsvjg.1" target="_blank" class="text-link">
              Zoom Link
            </a>
          </td>
        </tr>
        <tr>
          <td>Apr 21, 2026</td>
          <td><a href="https://zhenghaizhong.com/">Haizhong Zheng</a></td>
          <td>Efficient RL for LLMs</td>
          <td>Brian</td>
          <td onclick="event.stopPropagation()">
            <a href="https://illinois.zoom.us/j/81795451508?pwd=U3PAfk44ZtDJ2BaDJds2FXe2ACsvjg.1" target="_blank" class="text-link">
              Zoom Link
            </a>
          </td>
        </tr>
        <tr>
          <td>Apr 28, 2026</td>
          <td><a href="https://elisanguyen.github.io/">Elisa Nguyen</a></td>
          <td>TDA and Trustworthy AI</td>
          <td>Junwei</td>
          <td onclick="event.stopPropagation()">
            <a href="https://illinois.zoom.us/j/81795451508?pwd=U3PAfk44ZtDJ2BaDJds2FXe2ACsvjg.1" target="_blank" class="text-link">
              Zoom Link
            </a>
          </td>
        </tr>
      </tbody>
    </table>
  </div>

  <script>
    function toggleDetails(id) {
      const detailsRow = document.getElementById(id);
      const expandableRow = detailsRow.previousElementSibling;
      const indicator = expandableRow.querySelector('.expand-indicator');
      
      if (detailsRow.style.display === 'none') {
        detailsRow.style.display = 'table-row';
        indicator.textContent = '▲';
      } else {
        detailsRow.style.display = 'none';
        indicator.textContent = '▼';
      }
    }
  </script>

  <div class="calendar-note">
    <p><strong>Note:</strong> Times are provided in UTC and ET. Convert to your timezone before joining. Zoom links will be shared closer to the event date.</p>
  </div>

  <h2 class="section-title">📚 Past Seminars</h2>
  <div class="past-seminars">
    <table class="seminar-table">
      <thead>
        <tr>
          <th>Date</th>
          <th>Speaker</th>
          <th>Topic</th>
          <th>Host</th>
          <th>Recording</th>
        </tr>
      </thead>
      <tbody>
        <tr class="expandable-row" onclick="toggleDetails('past-seminar-1')">
          <td>Mar 3, 2026</td>
          <td><a href="https://dylanzsz.github.io/" onclick="event.stopPropagation()">Dylan Zhang</a></td>
          <td>More Fruitful SFT by Respecting The Learner's Distribution <span class="expand-indicator">▼</span></td>
          <td>Junwei</td>
          <td onclick="event.stopPropagation()">
            <a href="https://www.youtube.com/watch?v=_EXeM7qBiw0" target="_blank" class="text-link">
              YouTube
            </a>
          </td>
        </tr>
        <tr class="details-row" id="past-seminar-1" style="display: none;">
          <td colspan="5">
            <div class="seminar-details">
              <div class="speaker-photo">
                <img src="{{ '/assets/images/seminars/dylan-zhang.jpg' | relative_url }}" alt="Dylan Zhang">
              </div>
              <div class="seminar-content">
                <h3>More Fruitful SFT by Respecting The Learner's Distribution</h3>
                
                <h4>Abstract</h4>
                <p>Classic supervised fine-tuning (SFT) ignores the learner. It treats supervision as universally valid, even when the training data differs substantially from what the model itself would produce — a mismatch that has proven troublesome for LLM post-training in a variety of ways. Recent work on on-policy distillation and self-distillation fine-tuning has similarly argued that effective supervision must respect the learner's own policy.</p>
                
                <p>In this talk, I present two works built around that single principle: supervision should be aligned with the learner's distribution. Both implement it as a simple modification to standard SFT.</p>
                
                <p><strong>GRAPE</strong> addresses this from a data selection perspective. For each instruction, it selects the response with the highest probability under the target model from a pool of existing candidates, using only a forward pass. Models trained on GRAPE-curated data outperform multiple strong baselines while being lightweight and scalable.</p>
                
                <p>When SFT is followed by online RL, we show that stronger SFT (and variants) checkpoints can paradoxically underperform weaker ones after RL — because standard SFT optimizes for offline performance in isolation, without accounting for the on-policy distribution that RL will explore during its own rollouts.</p>
                
                <p><strong>PEAR</strong> extends this idea to the setting where SFT is followed by online RL. We first show that stronger SFT checkpoints can paradoxically underperform weaker ones after RL — because standard SFT optimizes for offline performance in isolation, without accounting for the on-policy distribution that RL will later explore. PEAR addresses this by reweighting the loss on each response according to its importance weight: how likely the target policy is to produce that response. We further show that this correction can operate at finer granularities, reweighting individual tokens based on how likely the continuation from that point in the offline data would be under the target policy. This importance-sampling correction, inspired by off-policy evaluation in RL, bridges the gap between the static SFT dataset and the dynamic on-policy distribution, yielding consistent post-RL gains.</p>
                
                <p>Both methods operationalize the same insight — that effective supervision must be shaped by the learner's own distribution — through complementary mechanisms: GRAPE by selecting responses the model trains on, PEAR by reweighting how much it learns. Together, they demonstrate that simple, policy-aware corrections can improve the effectiveness of SFT.</p>
                
                <h4>Bio</h4>
                <p>Dylan Zhang is a Ph.D. student in Computer Science at the University of Illinois Urbana-Champaign (UIUC), advised by Prof. Hao Peng. His research focuses on large language model (LLM) post-training, particularly on developing offline training algorithms for efficient and effective model alignment. More broadly, he is interested in understanding the behavior, generalization, and inductive biases of large language models—how they learn from data, adapt through supervision, and exhibit emergent capabilities.</p>
              </div>
            </div>
          </td>
        </tr>
        <tr class="expandable-row" onclick="toggleDetails('seminar-2')">
          <td>6 PM UTC | 2 PM ET<br>Mar 10, 2026</td>
          <td><a href="https://nick11roberts.science/" onclick="event.stopPropagation()">Nicholas Roberts</a></td>
          <td>Compute Optimal Scaling of Skills: Knowledge vs Reasoning <span class="expand-indicator">▼</span></td>
          <td>Brian</td>
          <td onclick="event.stopPropagation()">
            <a href="https://www.youtube.com/watch?v=qtuckPNS91Q" target="_blank" class="text-link">
              YouTube
            </a>
          </td>
        </tr>
        <tr class="details-row" id="seminar-2" style="display: none;">
          <td colspan="5">
            <div class="seminar-details">
              <div class="speaker-photo">
                <img src="{{ '/assets/images/seminars/nicholas-roberts.png' | relative_url }}" alt="Nicholas Roberts">
              </div>
              <div class="seminar-content">
                <h3>Compute Optimal Scaling of Skills: Knowledge vs Reasoning</h3>
                
                <h4>Abstract</h4>
                <p>Scaling laws are a critical component of the LLM development pipeline, most famously as a way to forecast training decisions such as 'compute-optimally' trading-off parameter count and dataset size, alongside a more recent growing list of other crucial decisions. In this work, we ask whether compute-optimal scaling behaviour can be skill-dependent. In particular, we examine knowledge and reasoning-based skills such as knowledge-based QA and code generation, and we answer this question in the affirmative: scaling laws are skill-dependent. Next, to understand whether skill-dependent scaling is an artefact of the pretraining datamix, we conduct an extensive ablation of different datamixes and find that, also when correcting for datamix differences, knowledge and code exhibit fundamental differences in scaling behaviour. We conclude with an analysis of how our findings relate to standard compute-optimal scaling using a validation set, and find that a misspecified validation set can impact compute-optimal parameter count by nearly 50%, depending on its skill composition.</p>
                
                <h4>Bio</h4>
                <p>Nicholas Roberts is a Ph.D. candidate in Computer Science at University of Wisconsin–Madison, advised by Frederic Sala in the Sprocket Lab, where he works on the science of foundation model scaling, data-efficiency, and adaptation to high-impact scientific domains---all with the ultimate goal of developing powerful scientific research agents. He has completed research internships at Meta's Llama team (working on scaling laws with Dieuwke Hupkes), Together AI (hybrid language models with Tri Dao), and Microsoft Research (Physics of AGI group with Sébastien Bubeck). He has received an honorable mention for the Jane Street Graduate Research Fellowship (2025) and was named an MLCommons Rising Star (2023). His academic path began at Fresno City College before earning his B.S. at UC San Diego where he worked with Sanjoy Dasgupta and Gary Cottrell and M.S. at Carnegie Mellon University with Ameet Talwalkar and Zack Lipton.</p>
              </div>
            </div>
          </td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="recordings-note">
    <p><em>We record talks when speakers consent. Recordings will be made available here.</em></p>
  </div>
</div>

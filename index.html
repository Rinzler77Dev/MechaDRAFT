<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Mecha Break Draft Helper</title>
<style>
  body { font-family: Arial, sans-serif; padding: 20px; }
  h2 { margin-top: 40px; }
  .section { margin-bottom: 30px; }
  .item-list { display: flex; flex-wrap: wrap; gap: 10px; }
  .item { padding: 8px 12px; border: 1px solid #ccc; border-radius: 4px; cursor: pointer; user-select: none; }
  .picked { background-color: #4caf50; color: white; }
  .banned { background-color: #f44336; color: white; }
  .summary { background: #eee; padding: 10px; border-radius: 5px; }
</style>
</head>
<body>

<h1>Mecha Break Draft Helper</h1>

<div class="section" id="maps-section">
  <h2>Map Picks</h2>
  <div>
    <strong>Available Maps:</strong>
    <div class="item-list" id="maps-list"></div>
  </div>
  <div style="margin-top: 10px;">
    <button id="pick-map-btn">Pick Map (Your Team)</button>
    <button id="ban-map-btn">Ban Map (Opponent)</button>
  </div>
</div>

<div class="section" id="strikers-section">
  <h2>Striker Bans</h2>
  <div class="item-list" id="strikers-list"></div>
  <button id="ban-striker-btn" style="margin-top: 10px;">Ban Striker</button>
</div>

<div class="section" id="summary-section">
  <h2>Draft Summary</h2>
  <div class="summary" id="draft-summary">
    <p><strong>Picked Maps:</strong> None</p>
    <p><strong>Banned Maps:</strong> None</p>
    <p><strong>Banned Strikers:</strong> None</p>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  // Sample data
  const maps = ['City Ruins', 'Frozen Tundra', 'Desert Outpost', 'Skyport', 'Lava Pit'];
  const strikers = ['Blaze', 'Frost', 'Shock', 'Vortex', 'Titan'];

  // State
  let mode = null; // 'pick-map', 'ban-map', 'ban-striker'
  let pickedMaps = [];
  let bannedMaps = [];
  let bannedStrikers = [];

  // Elements
  const mapsListEl = document.getElementById('maps-list');
  const strikersListEl = document.getElementById('strikers-list');
  const draftSummaryEl = document.getElementById('draft-summary');
  const pickMapBtn = document.getElementById('pick-map-btn');
  const banMapBtn = document.getElementById('ban-map-btn');
  const banStrikerBtn = document.getElementById('ban-striker-btn');

  function renderMaps() {
    mapsListEl.innerHTML = '';
    maps.forEach(map => {
      const div = document.createElement('div');
      div.className = 'item';
      if (pickedMaps.includes(map)) div.classList.add('picked');
      if (bannedMaps.includes(map)) div.classList.add('banned');
      div.textContent = map;
      div.onclick = () => {
        if (!mode) return alert('Select an action: Pick Map or Ban Map');
        if (mode === 'pick-map') {
          if (bannedMaps.includes(map)) return alert('Map is banned!');
          if (!pickedMaps.includes(map)) {
            pickedMaps.push(map);
          } else {
            pickedMaps = pickedMaps.filter(m => m !== map);
          }
        } else if (mode === 'ban-map') {
          if (pickedMaps.includes(map)) return alert('Map is picked!');
          if (!bannedMaps.includes(map)) {
            bannedMaps.push(map);
          } else {
            bannedMaps = bannedMaps.filter(m => m !== map);
          }
        }
        updateSummary();
        renderMaps();
      };
      mapsListEl.appendChild(div);
    });
  }

  function renderStrikers() {
    strikersListEl.innerHTML = '';
    strikers.forEach(striker => {
      const div = document.createElement('div');
      div.className = 'item';
      if (bannedStrikers.includes(striker)) div.classList.add('banned');
      div.textContent = striker;
      div.onclick = () => {
        if (mode !== 'ban-striker') return alert('Select "Ban Striker" to ban.');
        if (!bannedStrikers.includes(striker)) {
          bannedStrikers.push(striker);
        } else {
          bannedStrikers = bannedStrikers.filter(s => s !== striker);
        }
        updateSummary();
        renderStrikers();
      };
      strikersListEl.appendChild(div);
    });
  }

  function updateSummary() {
    draftSummaryEl.innerHTML = `
      <p><strong>Picked Maps:</strong> ${pickedMaps.length ? pickedMaps.join(', ') : 'None'}</p>
      <p><strong>Banned Maps:</strong> ${bannedMaps.length ? bannedMaps.join(', ') : 'None'}</p>
      <p><strong>Banned Strikers:</strong> ${bannedStrikers.length ? bannedStrikers.join(', ') : 'None'}</p>
    `;
  }

  pickMapBtn.onclick = () => { mode = 'pick-map'; alert('Click maps to pick for your team'); };
  banMapBtn.onclick = () => { mode = 'ban-map'; alert('Click maps to ban for opponent'); };
  banStrikerBtn.onclick = () => { mode = 'ban-striker'; alert('Click strikers to ban'); };

  // Initial render
  renderMaps();
  renderStrikers();
  updateSummary();
});
</script>

</body>
</html>

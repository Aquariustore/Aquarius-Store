<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aquarius Store — Admin</title>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700&family=Manrope:wght@400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<style>
  :root{
    --ink:#111111;
    --white:#ffffff;
    --sand:#fafafa;
    --line:rgba(0,0,0,0.14);
    --danger:#b02a2a;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    font-family:'Manrope',sans-serif;
    background:var(--sand);
    color:var(--ink);
  }
  h1,h2,.display{ font-family:'Fraunces',serif; }

  header{
    padding:20px;
    background:#000;
    color:var(--white);
    display:flex;
    justify-content:space-between;
    align-items:center;
  }
  header h1{ font-size:20px; margin:0; }
  header button{
    background:transparent;
    border:1px solid rgba(255,255,255,0.4);
    color:var(--white);
    padding:6px 12px;
    border-radius:8px;
    font-size:12px;
    cursor:pointer;
  }

  .wrap{ max-width:720px; margin:0 auto; padding:20px; }

  /* LOGIN */
  .login-box{
    max-width:340px;
    margin:60px auto;
    text-align:center;
    padding:40px 24px;
    background:#000;
    border-radius:18px;
    color:#fff;
  }
  .login-box p{ color:rgba(255,255,255,0.65); font-size:13px; margin-top:0; margin-bottom:20px; }
  .login-box input{ margin-bottom:10px; }
  input, select{
    width:100%;
    padding:12px 14px;
    border-radius:10px;
    border:1px solid var(--line);
    font-size:14px;
    font-family:'Manrope',sans-serif;
    background:var(--white);
    color:var(--ink);
    margin-bottom:10px;
  }
  .btn{
    width:100%;
    padding:13px;
    border-radius:10px;
    border:none;
    background:#000;
    color:#fff;
    font-size:14px;
    font-weight:700;
    cursor:pointer;
  }
  .btn.secondary{
    background:transparent;
    border:1px solid var(--ink);
    color:var(--ink);
  }
  .btn.danger{
    background:var(--danger);
  }
  .login-box .btn{ background:#fff; color:#000; }
  .error-msg{
    color:var(--danger);
    font-size:12.5px;
    margin-top:-4px;
    margin-bottom:10px;
    display:none;
  }

  /* TABS */
  .section-tabs{
    display:flex;
    gap:8px;
    margin:20px 0;
  }
  .section-tab{
    padding:8px 16px;
    border-radius:999px;
    border:1px solid var(--line);
    background:var(--white);
    font-size:13px;
    font-weight:600;
    cursor:pointer;
  }
  .section-tab.active{ background:#000; color:#fff; border-color:#000; }

  .card-box{
    background:var(--white);
    border:1px solid var(--line);
    border-radius:14px;
    padding:16px;
    margin-bottom:16px;
  }
  .card-box h2{ font-size:16px; margin:0 0 12px; }

  label{ font-size:12px; font-weight:600; color:#555; display:block; margin-bottom:4px; }
  .field{ margin-bottom:12px; }

  /* PRODUCT LIST */
  .product-row{
    display:flex;
    gap:12px;
    align-items:center;
    padding:12px 0;
    border-bottom:1px solid var(--line);
  }
  .product-thumb{
    width:56px;height:56px;
    border-radius:8px;
    object-fit:cover;
    background:#eee;
    flex:none;
  }
  .product-info{ flex:1; min-width:0; }
  .product-name{ font-size:13.5px; font-weight:600; }
  .product-sub{ font-size:12px; color:#777; }
  .product-actions{ display:flex; gap:6px; flex:none; }
  .icon-btn{
    border:1px solid var(--line);
    background:var(--white);
    border-radius:8px;
    padding:6px 10px;
    font-size:12px;
    cursor:pointer;
  }
  .stock-input{
    width:60px;
    padding:6px;
    text-align:center;
    border-radius:6px;
    border:1px solid var(--line);
    margin-bottom:0;
  }
  .inactive-tag{
    font-size:11px;
    color:#999;
    font-weight:700;
    margin-left:6px;
  }

  /* SALES LIST */
  .sale-row{
    padding:12px 0;
    border-bottom:1px solid var(--line);
  }
  .sale-top{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;
    gap:10px;
    margin-bottom:8px;
  }
  .sale-info{ flex:1; min-width:0; }
  .sale-name{ font-size:13.5px; font-weight:600; }
  .sale-sub{ font-size:12px; color:#777; }
  .sale-items{ font-size:12.5px; color:#444; margin:6px 0; }
  .sale-items div{ padding:2px 0; }
  .sale-total{ font-size:14px; font-weight:700; margin-top:4px; }
  .sale-controls{
    display:flex;
    gap:8px;
    flex-wrap:wrap;
  }
  .sale-controls select{
    width:auto;
    margin-bottom:0;
    font-size:12px;
    padding:6px 8px;
  }
  .cart-row{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:8px 0;
    border-bottom:1px solid var(--line);
    font-size:13px;
  }
  .cart-total-box{
    display:flex;
    justify-content:space-between;
    font-weight:700;
    font-size:15px;
    padding:10px 0;
  }
  #toast{
    position:fixed;
    bottom:20px; left:50%; transform:translateX(-50%);
    background:#000; color:#fff;
    padding:10px 18px; border-radius:8px;
    font-size:13px; display:none; z-index:50;
  }
</style>
</head>
<body>

<div id="loginScreen" class="login-box">
  <p>Área administrativa</p>
  <div class="field">
    <input type="password" id="passwordInput" placeholder="Senha de acesso">
  </div>
  <p class="error-msg" id="loginError">Senha incorreta.</p>
  <button class="btn" onclick="tryLogin()">Entrar</button>
</div>

<div id="adminScreen" style="display:none;">
  <header>
    <div style="display:flex;align-items:center;gap:10px;">
      <h1>Admin</h1>
    </div>
    <button onclick="logout()">Sair</button>
  </header>

  <div class="wrap">
    <div class="section-tabs">
      <div class="section-tab active" id="tabProducts" onclick="showSection('products')">Produtos</div>
      <div class="section-tab" id="tabSales" onclick="showSection('sales')">Vendas</div>
      <div class="section-tab" id="tabSettings" onclick="showSection('settings')">Configurações</div>
    </div>

    <!-- PRODUCTS SECTION -->
    <div id="sectionProducts">
      <div class="card-box">
        <h2 id="formTitle">Novo produto</h2>
        <div class="field">
          <label>Nome do produto</label>
          <input type="text" id="pName" placeholder="Ex: Vestido midi linho">
        </div>
        <div class="field">
          <label>Categoria</label>
          <select id="pCategory" onchange="toggleSubcategoryField()">
            <option value="Moda feminina">Moda feminina</option>
            <option value="Moda infantil">Moda infantil</option>
            <option value="Casa, mesa e banho">Casa, mesa e banho</option>
          </select>
        </div>
        <div class="field" id="subcategoryField" style="display:none;">
          <label>Subcategoria</label>
          <select id="pSubcategory"></select>
        </div>
        <div class="field">
          <label>Preço (R$)</label>
          <input type="number" id="pPrice" step="0.01" placeholder="Ex: 129.90">
        </div>
        <div class="field" style="display:flex;align-items:center;gap:8px;">
          <input type="checkbox" id="pHasColors" onchange="toggleColorMode()" style="width:auto;margin:0;">
          <label style="margin:0;">Esse produto tem cores diferentes?</label>
        </div>
        <div class="field" id="simpleStockField">
          <label>Estoque (quantidade)</label>
          <input type="number" id="pStock" step="1" placeholder="Ex: 5">
        </div>
        <div class="field" id="colorStockField" style="display:none;">
          <label>Cores e estoque de cada uma</label>
          <div id="colorRows"></div>
          <button type="button" class="icon-btn" onclick="addColorRow()">+ Adicionar cor</button>
        </div>
        <div class="field">
          <label>Descrição do produto</label>
          <textarea id="pDescription" rows="3" placeholder="Detalhes, tecido, medidas, etc." style="width:100%;padding:12px 14px;border-radius:10px;border:1px solid var(--line);font-family:'Manrope',sans-serif;font-size:14px;resize:vertical;"></textarea>
        </div>
        <div class="field">
          <label>Foto do produto</label>
          <input type="file" id="pImage" accept="image/*">
        </div>
        <input type="hidden" id="pId">
        <input type="hidden" id="pExistingImage">
        <button class="btn" id="saveBtn" onclick="saveProduct()">Salvar produto</button>
        <button class="btn secondary" id="cancelEditBtn" style="display:none;margin-top:8px;" onclick="resetForm()">Cancelar edição</button>
      </div>

      <div class="card-box">
        <h2>Produtos cadastrados</h2>
        <div id="productList">Carregando...</div>
      </div>
    </div>

    <!-- SALES SECTION -->
    <div id="sectionSales" style="display:none;">
      <div class="card-box">
        <h2>Registrar venda</h2>
        <div class="field">
          <label>Produto</label>
          <select id="saleProduct" onchange="onSaleProductChange()"></select>
        </div>
        <div class="field" id="saleColorField" style="display:none;">
          <label>Cor</label>
          <select id="saleColor"></select>
        </div>
        <div class="field">
          <label>Quantidade</label>
          <input type="number" id="saleQuantity" min="1" step="1" value="1">
        </div>
        <button type="button" class="btn secondary" onclick="addCartItem()">+ Adicionar item à venda</button>

        <div id="cartItemsBox" style="margin-top:14px;display:none;">
          <div id="cartRows"></div>
          <div class="cart-total-box">
            <span>Total da venda</span>
            <span id="cartTotalValue">R$ 0,00</span>
          </div>
        </div>

        <div class="field" style="margin-top:14px;">
          <label>Nome do cliente</label>
          <input type="text" id="saleClient" placeholder="Ex: Maria Silva">
        </div>
        <div class="field">
          <label>Conta</label>
          <select id="saleAccount">
            <option value="Thamirys">Thamirys</option>
            <option value="Renata">Renata</option>
          </select>
        </div>
        <div class="field">
          <label>Status de entrega</label>
          <select id="saleDeliveryStatus">
            <option value="Reservado">Reservado</option>
            <option value="Entregue">Entregue</option>
          </select>
        </div>
        <div class="field">
          <label>Status de pagamento</label>
          <select id="salePaymentStatus">
            <option value="Pendente">Pendente</option>
            <option value="Pago">Pago</option>
          </select>
        </div>
        <button class="btn" id="saveSaleBtn" onclick="saveSale()">Registrar venda</button>
      </div>

      <div class="card-box">
        <h2>Histórico de vendas</h2>
        <div style="display:flex;gap:8px;margin-bottom:14px;flex-wrap:wrap;">
          <select id="filterPayment" onchange="applyFilters()" style="width:auto;margin-bottom:0;">
            <option value="all">Pagamento: Todos</option>
            <option value="Pago">Pago</option>
            <option value="Pendente">Pendente</option>
          </select>
          <select id="filterDelivery" onchange="applyFilters()" style="width:auto;margin-bottom:0;">
            <option value="all">Entrega: Todos</option>
            <option value="Entregue">Entregue</option>
            <option value="Reservado">Reservado</option>
          </select>
        </div>
        <div id="salesSummary" style="background:var(--sand);border-radius:10px;padding:12px;margin-bottom:14px;font-size:13.5px;"></div>
        <div id="salesList">Carregando...</div>
      </div>
    </div>

    <!-- SETTINGS SECTION -->
    <div id="sectionSettings" style="display:none;">
      <div class="card-box">
        <h2>Trocar senha do admin</h2>
        <div class="field">
          <label>Senha atual</label>
          <input type="password" id="currentPass">
        </div>
        <div class="field">
          <label>Nova senha</label>
          <input type="password" id="newPass">
        </div>
        <p class="error-msg" id="passError">Senha atual incorreta.</p>
        <button class="btn" onclick="changePassword()">Atualizar senha</button>
      </div>

      <div class="card-box">
        <h2>Subcategorias de "Casa, mesa e banho"</h2>
        <div id="subcategoryList" style="margin-bottom:14px;"></div>
        <div class="field" style="display:flex;gap:8px;">
          <input type="text" id="newSubcategoryName" placeholder="Nova subcategoria (ex: Tapetes)" style="margin-bottom:0;">
          <button class="btn" style="width:auto;padding:12px 18px;" onclick="addSubcategory()">Adicionar</button>
        </div>
      </div>
    </div>
  </div>
</div>

<div id="toast"></div>

<script>
const SUPABASE_URL = "https://qrbszabxipsmmzjrpcrd.supabase.co";
const SUPABASE_KEY = "sb_publishable_gYkQcuXvc2VGsonYMz3HiQ_hMWvSICg";
const sb = supabase.createClient(SUPABASE_URL, SUPABASE_KEY);

let products = [];
let subcategories = [];
let cartItems = []; // { productId, productName, quantity, unitPrice }
let allSales = [];

async function loadSubcategories(){
  const { data, error } = await sb.from('subcategories').select('*').eq('category', 'Casa, mesa e banho').order('name');
  if(error){ console.error(error); return; }
  subcategories = data || [];
  populateSubcategorySelect();
  renderSubcategoryList();
}

function populateSubcategorySelect(keepValue){
  const select = document.getElementById('pSubcategory');
  const current = keepValue !== undefined ? keepValue : select.value;
  select.innerHTML = subcategories.map(s => `<option value="${s.name}">${s.name}</option>`).join('');
  if(current){
    const exists = subcategories.some(s => s.name === current);
    if(!exists){
      const opt = document.createElement('option');
      opt.value = current;
      opt.textContent = `${current} (removida)`;
      select.appendChild(opt);
    }
    select.value = current;
  }
}

function renderSubcategoryList(){
  const el = document.getElementById('subcategoryList');
  if(subcategories.length === 0){
    el.innerHTML = '<p style="font-size:13px;color:#888;">Nenhuma subcategoria cadastrada.</p>';
    return;
  }
  el.innerHTML = subcategories.map(s => `
    <div style="display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:1px solid var(--line);">
      <span style="font-size:13.5px;">${s.name}</span>
      <button class="icon-btn" onclick="deleteSubcategory('${s.id}')">Excluir</button>
    </div>
  `).join('');
}

async function addSubcategory(){
  const input = document.getElementById('newSubcategoryName');
  const name = input.value.trim();
  if(!name){ showToast('Digite o nome da subcategoria'); return; }
  const { error } = await sb.from('subcategories').insert({ category: 'Casa, mesa e banho', name });
  if(error){ showToast('Erro ao adicionar'); console.error(error); return; }
  input.value = '';
  showToast('Subcategoria adicionada');
  loadSubcategories();
}

async function deleteSubcategory(id){
  if(!confirm('Excluir essa subcategoria? Produtos que já usam ela mantêm o texto salvo, mas ela some da lista de opções.')) return;
  const { error } = await sb.from('subcategories').delete().eq('id', id);
  if(error){ showToast('Erro ao excluir'); return; }
  showToast('Subcategoria excluída');
  loadSubcategories();
}

function showToast(msg, detail){
  const t = document.getElementById('toast');
  t.textContent = detail ? `${msg}: ${detail}` : msg;
  t.style.display = 'block';
  setTimeout(()=> t.style.display='none', detail ? 6000 : 2500);
}

function formatMoney(v){
  return 'R$ ' + Number(v).toFixed(2).replace('.', ',');
}

/* ---------- LOGIN ---------- */
async function tryLogin(){
  const input = document.getElementById('passwordInput').value.trim();
  const { data, error } = await sb.from('admin_config').select('password').eq('id', 1).single();
  if(error || !data){
    document.getElementById('loginError').style.display = 'block';
    return;
  }
  if(input === data.password){
    sessionStorage.setItem('aquarius_admin', 'true');
    document.getElementById('loginScreen').style.display = 'none';
    document.getElementById('adminScreen').style.display = 'block';
    loadProducts();
    loadSubcategories();
  } else {
    document.getElementById('loginError').style.display = 'block';
  }
}

function logout(){
  sessionStorage.removeItem('aquarius_admin');
  document.getElementById('adminScreen').style.display = 'none';
  document.getElementById('loginScreen').style.display = 'block';
  document.getElementById('passwordInput').value = '';
}

if(sessionStorage.getItem('aquarius_admin') === 'true'){
  document.getElementById('loginScreen').style.display = 'none';
  document.getElementById('adminScreen').style.display = 'block';
  loadProducts();
  loadSubcategories();
}

/* ---------- SECTION TABS ---------- */
function showSection(section){
  document.getElementById('sectionProducts').style.display = section==='products' ? 'block' : 'none';
  document.getElementById('sectionSales').style.display = section==='sales' ? 'block' : 'none';
  document.getElementById('sectionSettings').style.display = section==='settings' ? 'block' : 'none';
  document.getElementById('tabProducts').classList.toggle('active', section==='products');
  document.getElementById('tabSales').classList.toggle('active', section==='sales');
  document.getElementById('tabSettings').classList.toggle('active', section==='settings');
  if(section === 'sales'){
    populateSaleProductSelect();
    loadSales();
  }
}

function toggleSubcategoryField(){
  const isCasa = document.getElementById('pCategory').value === 'Casa, mesa e banho';
  document.getElementById('subcategoryField').style.display = isCasa ? 'block' : 'none';
}

/* ---------- COLOR VARIANTS ---------- */
function toggleColorMode(){
  const hasColors = document.getElementById('pHasColors').checked;
  document.getElementById('simpleStockField').style.display = hasColors ? 'none' : 'block';
  document.getElementById('colorStockField').style.display = hasColors ? 'block' : 'none';
  if(hasColors && document.getElementById('colorRows').children.length === 0){
    addColorRow();
  }
}

function addColorRow(color, stock){
  const el = document.getElementById('colorRows');
  const row = document.createElement('div');
  row.style.cssText = 'display:flex;gap:8px;margin-bottom:8px;align-items:center;';
  row.innerHTML = `
    <input type="text" placeholder="Cor (ex: Preto)" class="color-name" style="margin-bottom:0;flex:2;" value="${color||''}">
    <input type="number" placeholder="Estoque" class="color-stock" style="margin-bottom:0;flex:1;" value="${stock!=null?stock:''}">
    <button type="button" class="icon-btn" onclick="this.parentElement.remove()">✕</button>
  `;
  el.appendChild(row);
}

function getColorRowsData(){
  const rows = document.querySelectorAll('#colorRows > div');
  const result = [];
  rows.forEach(row => {
    const name = row.querySelector('.color-name').value.trim();
    const stock = parseInt(row.querySelector('.color-stock').value, 10);
    if(name && !isNaN(stock)) result.push({ color: name, stock });
  });
  return result;
}

/* ---------- PRODUCTS ---------- */
async function loadProducts(){
  const { data, error } = await sb.from('products').select('*').order('created_at', {ascending:false});
  if(error){ showToast('Erro ao carregar produtos'); console.error(error); return; }
  products = data || [];

  const { data: variantData, error: variantError } = await sb.from('product_variants').select('*');
  if(!variantError && variantData){
    products.forEach(p => {
      p.variants = variantData.filter(v => v.product_id === p.id);
    });
  }

  renderProductList();
}

function renderProductList(){
  const el = document.getElementById('productList');
  if(products.length === 0){
    el.innerHTML = '<p style="font-size:13px;color:#888;">Nenhum produto cadastrado ainda.</p>';
    return;
  }
  el.innerHTML = products.map(p => {
    const hasVariants = p.variants && p.variants.length > 0;
    const stockControl = hasVariants
      ? `<div style="font-size:11px;color:#555;text-align:right;">${p.variants.map(v => `${v.color}: <input type="number" style="width:40px;padding:2px;text-align:center;border-radius:4px;border:1px solid var(--line);margin:0 2px;" value="${v.stock}" onchange="updateVariantStock('${v.id}', this.value)">`).join('<br>')}</div>`
      : `<input type="number" class="stock-input" value="${p.stock}" onchange="updateStock('${p.id}', this.value)">`;
    return `
    <div class="product-row">
      <img class="product-thumb" src="${p.image_url || ''}" onerror="this.style.background='#eee'; this.src='';">
      <div class="product-info">
        <div class="product-name">${p.name} ${!p.active ? '<span class=\"inactive-tag\">INATIVO</span>' : ''}</div>
        <div class="product-sub">${p.category}${p.subcategory ? ' • '+p.subcategory : ''} • ${formatMoney(p.price)}</div>
      </div>
      ${stockControl}
      <div class="product-actions">
        <button class="icon-btn" onclick="editProduct('${p.id}')">Editar</button>
        <button class="icon-btn" onclick="toggleActive('${p.id}', ${p.active})">${p.active ? 'Ocultar' : 'Ativar'}</button>
        <button class="icon-btn" onclick="deleteProduct('${p.id}')">Excluir</button>
      </div>
    </div>
  `;
  }).join('');
}

async function updateStock(id, value){
  const stock = parseInt(value, 10);
  if(isNaN(stock) || stock < 0){ showToast('Quantidade inválida'); return; }
  const { error } = await sb.from('products').update({ stock }).eq('id', id);
  if(error){ showToast('Erro ao atualizar estoque'); return; }
  const p = products.find(x=>x.id===id);
  if(p) p.stock = stock;
  showToast('Estoque atualizado');
}

async function updateVariantStock(variantId, value){
  const stock = parseInt(value, 10);
  if(isNaN(stock) || stock < 0){ showToast('Quantidade inválida'); return; }
  const { error } = await sb.from('product_variants').update({ stock }).eq('id', variantId);
  if(error){ showToast('Erro ao atualizar estoque'); return; }
  showToast('Estoque atualizado');
}

async function toggleActive(id, current){
  const { error } = await sb.from('products').update({ active: !current }).eq('id', id);
  if(error){ showToast('Erro ao atualizar'); return; }
  loadProducts();
}

async function deleteProduct(id){
  if(!confirm('Tem certeza que quer excluir esse produto? Essa ação não pode ser desfeita.')) return;
  const { error } = await sb.from('products').delete().eq('id', id);
  if(error){ showToast('Erro ao excluir'); return; }
  showToast('Produto excluído');
  loadProducts();
}

function editProduct(id){
  const p = products.find(x=>x.id===id);
  if(!p) return;
  document.getElementById('formTitle').textContent = 'Editar produto';
  document.getElementById('pId').value = p.id;
  document.getElementById('pName').value = p.name;
  document.getElementById('pCategory').value = p.category;
  toggleSubcategoryField();
  if(p.category === 'Casa, mesa e banho'){
    populateSubcategorySelect(p.subcategory || '');
  }
  document.getElementById('pPrice').value = p.price;
  document.getElementById('pDescription').value = p.description || '';
  document.getElementById('pExistingImage').value = p.image_url || '';
  document.getElementById('cancelEditBtn').style.display = 'block';

  const hasVariants = p.variants && p.variants.length > 0;
  document.getElementById('pHasColors').checked = hasVariants;
  document.getElementById('colorRows').innerHTML = '';
  if(hasVariants){
    p.variants.forEach(v => addColorRow(v.color, v.stock));
    document.getElementById('pStock').value = '';
  } else {
    document.getElementById('pStock').value = p.stock;
  }
  toggleColorMode();

  window.scrollTo({top:0, behavior:'smooth'});
}

function resetForm(){
  document.getElementById('formTitle').textContent = 'Novo produto';
  document.getElementById('pId').value = '';
  document.getElementById('pName').value = '';
  document.getElementById('pCategory').value = 'Moda feminina';
  toggleSubcategoryField();
  document.getElementById('pPrice').value = '';
  document.getElementById('pDescription').value = '';
  document.getElementById('pStock').value = '';
  document.getElementById('pImage').value = '';
  document.getElementById('pExistingImage').value = '';
  document.getElementById('pHasColors').checked = false;
  document.getElementById('colorRows').innerHTML = '';
  toggleColorMode();
  document.getElementById('cancelEditBtn').style.display = 'none';
}

async function saveProduct(){
  const id = document.getElementById('pId').value;
  const name = document.getElementById('pName').value.trim();
  const category = document.getElementById('pCategory').value;
  const subcategory = category === 'Casa, mesa e banho' ? document.getElementById('pSubcategory').value : null;
  const price = parseFloat(document.getElementById('pPrice').value);
  const description = document.getElementById('pDescription').value.trim() || null;
  const hasColors = document.getElementById('pHasColors').checked;
  const colorRows = hasColors ? getColorRowsData() : [];
  const stock = hasColors ? colorRows.reduce((sum, c) => sum + c.stock, 0) : parseInt(document.getElementById('pStock').value, 10);
  const file = document.getElementById('pImage').files[0];
  let imageUrl = document.getElementById('pExistingImage').value || null;

  if(!name || !category || isNaN(price) || isNaN(stock)){
    showToast('Preencha todos os campos obrigatórios');
    return;
  }
  if(category === 'Casa, mesa e banho' && !subcategory){
    showToast('Cadastre uma subcategoria em Configurações antes de salvar, ou selecione uma');
    return;
  }
  if(hasColors && colorRows.length === 0){
    showToast('Adicione pelo menos uma cor com estoque');
    return;
  }

  document.getElementById('saveBtn').textContent = 'Salvando...';
  document.getElementById('saveBtn').disabled = true;

  if(file){
    const ext = file.name.split('.').pop();
    const fileName = `${Date.now()}_${Math.random().toString(36).slice(2)}.${ext}`;
    const { error: uploadError } = await sb.storage.from('product-images').upload(fileName, file);
    if(uploadError){
      showToast('Erro ao enviar foto', uploadError.message);
      document.getElementById('saveBtn').textContent = 'Salvar produto';
      document.getElementById('saveBtn').disabled = false;
      console.error(uploadError);
      return;
    }
    const { data: urlData } = sb.storage.from('product-images').getPublicUrl(fileName);
    imageUrl = urlData.publicUrl;
  }

  const payload = { name, category, subcategory, price, stock, image_url: imageUrl, description };

  let error, productId = id;
  if(id){
    ({ error } = await sb.from('products').update(payload).eq('id', id));
  } else {
    payload.active = true;
    const { data: inserted, error: insertError } = await sb.from('products').insert(payload).select().single();
    error = insertError;
    if(inserted) productId = inserted.id;
  }

  if(error){
    document.getElementById('saveBtn').textContent = 'Salvar produto';
    document.getElementById('saveBtn').disabled = false;
    showToast('Erro ao salvar produto', error.message);
    console.error(error);
    return;
  }

  // Sync color variants: remove old ones, insert current set
  if(productId){
    await sb.from('product_variants').delete().eq('product_id', productId);
    if(hasColors && colorRows.length > 0){
      const variantPayload = colorRows.map(c => ({ product_id: productId, color: c.color, stock: c.stock }));
      const { error: variantError } = await sb.from('product_variants').insert(variantPayload);
      if(variantError){ console.error(variantError); showToast('Produto salvo, mas houve erro nas cores'); }
    }
  }

  document.getElementById('saveBtn').textContent = 'Salvar produto';
  document.getElementById('saveBtn').disabled = false;

  showToast('Produto salvo com sucesso');
  resetForm();
  loadProducts();
}

/* ---------- SALES / CART ---------- */
function populateSaleProductSelect(){
  const select = document.getElementById('saleProduct');
  const current = select.value;
  select.innerHTML = products
    .filter(p => p.active)
    .map(p => `<option value="${p.id}">${p.name} — ${formatMoney(p.price)}</option>`)
    .join('');
  if(current) select.value = current;
  onSaleProductChange();
}

function onSaleProductChange(){
  const productId = document.getElementById('saleProduct').value;
  const product = products.find(p => p.id === productId);
  const colorField = document.getElementById('saleColorField');
  const colorSelect = document.getElementById('saleColor');

  if(product && product.variants && product.variants.length > 0){
    colorField.style.display = 'block';
    colorSelect.innerHTML = product.variants
      .map(v => `<option value="${v.id}">${v.color} (estoque: ${v.stock})</option>`)
      .join('');
  } else {
    colorField.style.display = 'none';
    colorSelect.innerHTML = '';
  }
}

function addCartItem(){
  const productId = document.getElementById('saleProduct').value;
  const quantity = parseInt(document.getElementById('saleQuantity').value, 10);
  const product = products.find(p => p.id === productId);

  if(!product){ showToast('Selecione um produto'); return; }
  if(isNaN(quantity) || quantity < 1){ showToast('Quantidade inválida'); return; }

  const hasVariants = product.variants && product.variants.length > 0;
  let variantId = null, color = null, availableStock = product.stock;

  if(hasVariants){
    variantId = document.getElementById('saleColor').value;
    const variant = product.variants.find(v => v.id === variantId);
    if(!variant){ showToast('Selecione uma cor'); return; }
    color = variant.color;
    availableStock = variant.stock;
  }

  const alreadyInCart = cartItems
    .filter(c => c.productId === productId && c.variantId === variantId)
    .reduce((s,c)=>s+c.quantity,0);

  if(quantity + alreadyInCart > availableStock){
    showToast(`Estoque insuficiente (disponível: ${availableStock})`);
    return;
  }

  const existing = cartItems.find(c => c.productId === productId && c.variantId === variantId);
  if(existing){
    existing.quantity += quantity;
  } else {
    cartItems.push({ productId, productName: product.name, quantity, unitPrice: Number(product.price), variantId, color });
  }

  document.getElementById('saleQuantity').value = 1;
  renderCart();
}

function removeCartItem(index){
  cartItems.splice(index, 1);
  renderCart();
}

function renderCart(){
  const box = document.getElementById('cartItemsBox');
  const rows = document.getElementById('cartRows');
  if(cartItems.length === 0){
    box.style.display = 'none';
    rows.innerHTML = '';
    document.getElementById('cartTotalValue').textContent = formatMoney(0);
    return;
  }
  box.style.display = 'block';
  rows.innerHTML = cartItems.map((c, i) => `
    <div class="cart-row">
      <span>${c.productName}${c.color ? ' ('+c.color+')' : ''} × ${c.quantity}</span>
      <span style="display:flex;align-items:center;gap:10px;">
        ${formatMoney(c.unitPrice * c.quantity)}
        <button type="button" class="icon-btn" onclick="removeCartItem(${i})">✕</button>
      </span>
    </div>
  `).join('');
  const total = cartItems.reduce((sum, c) => sum + c.unitPrice * c.quantity, 0);
  document.getElementById('cartTotalValue').textContent = formatMoney(total);
}

async function saveSale(){
  if(cartItems.length === 0){
    showToast('Adicione pelo menos um item à venda');
    return;
  }

  const clientName = document.getElementById('saleClient').value.trim() || null;
  const account = document.getElementById('saleAccount').value;
  const deliveryStatus = document.getElementById('saleDeliveryStatus').value;
  const paymentStatus = document.getElementById('salePaymentStatus').value;

  // double-check stock right before saving
  for(const item of cartItems){
    const product = products.find(p => p.id === item.productId);
    if(!product){ showToast(`Produto não encontrado: ${item.productName}`); return; }
    if(item.variantId){
      const variant = product.variants.find(v => v.id === item.variantId);
      if(!variant || item.quantity > variant.stock){
        showToast(`Estoque insuficiente para ${item.productName} (${item.color})`);
        return;
      }
    } else if(item.quantity > product.stock){
      showToast(`Estoque insuficiente para ${item.productName}`);
      return;
    }
  }

  document.getElementById('saveSaleBtn').textContent = 'Salvando...';
  document.getElementById('saveSaleBtn').disabled = true;

  const saleGroup = `${Date.now()}_${Math.random().toString(36).slice(2)}`;

  const rows = cartItems.map(item => ({
    product_id: item.productId,
    product_name: item.productName,
    quantity: item.quantity,
    unit_price: item.unitPrice,
    color: item.color,
    sale_group: saleGroup,
    client_name: clientName,
    account,
    delivery_status: deliveryStatus,
    payment_status: paymentStatus
  }));

  const { error: saleError } = await sb.from('sales').insert(rows);

  if(saleError){
    showToast('Erro ao registrar venda', saleError.message);
    console.error(saleError);
    document.getElementById('saveSaleBtn').textContent = 'Registrar venda';
    document.getElementById('saveSaleBtn').disabled = false;
    return;
  }

  for(const item of cartItems){
    const product = products.find(p => p.id === item.productId);
    if(item.variantId){
      const variant = product.variants.find(v => v.id === item.variantId);
      const newVariantStock = variant.stock - item.quantity;
      const { error: variantError } = await sb.from('product_variants').update({ stock: newVariantStock }).eq('id', item.variantId);
      if(!variantError){
        variant.stock = newVariantStock;
        const newTotalStock = product.variants.reduce((s,v)=>s+v.stock, 0);
        const { error: stockError } = await sb.from('products').update({ stock: newTotalStock }).eq('id', item.productId);
        if(!stockError) product.stock = newTotalStock;
      }
    } else {
      const newStock = product.stock - item.quantity;
      const { error: stockError } = await sb.from('products').update({ stock: newStock }).eq('id', item.productId);
      if(!stockError) product.stock = newStock;
    }
  }

  document.getElementById('saveSaleBtn').textContent = 'Registrar venda';
  document.getElementById('saveSaleBtn').disabled = false;
  document.getElementById('saleClient').value = '';
  cartItems = [];
  renderCart();

  showToast('Venda registrada com sucesso');
  populateSaleProductSelect();
  loadSales();
}


async function loadSales(){
  const { data, error } = await sb.from('sales').select('*').order('created_at', {ascending:false});
  if(error){ showToast('Erro ao carregar vendas', error.message); console.error(error); return; }
  allSales = data || [];
  applyFilters();
}

function applyFilters(){
  const payment = document.getElementById('filterPayment').value;
  const delivery = document.getElementById('filterDelivery').value;
  let filtered = allSales;
  if(payment !== 'all') filtered = filtered.filter(s => s.payment_status === payment);
  if(delivery !== 'all') filtered = filtered.filter(s => s.delivery_status === delivery);
  renderSalesSummary(filtered);
  renderSalesList(filtered);
}

function renderSalesSummary(rows){
  const el = document.getElementById('salesSummary');
  if(rows.length === 0){
    el.innerHTML = '<span style="color:#888;">Nenhuma venda nesse filtro.</span>';
    return;
  }
  const groups = groupSales(rows);
  let total = 0;
  const byAccount = {};
  groups.forEach(g => {
    const hasPrices = g.items.every(i => i.unit_price != null);
    if(hasPrices){
      const groupTotal = g.items.reduce((s,i)=> s + Number(i.unit_price) * i.quantity, 0);
      total += groupTotal;
      byAccount[g.account] = (byAccount[g.account] || 0) + groupTotal;
    }
  });
  const accountsHtml = Object.keys(byAccount)
    .map(acc => `<div>Caixa ${acc}: <strong>${formatMoney(byAccount[acc])}</strong></div>`)
    .join('');
  el.innerHTML = `<div style="font-size:15px;font-weight:700;margin-bottom:6px;">Total: ${formatMoney(total)}</div>${accountsHtml}`;
}

function groupSales(sales){
  const groups = [];
  const byGroup = {};
  sales.forEach(s => {
    const key = s.sale_group || s.id; // vendas antigas sem grupo viram grupo de 1 item
    if(!byGroup[key]){
      byGroup[key] = { key, created_at: s.created_at, client_name: s.client_name, account: s.account,
        delivery_status: s.delivery_status, payment_status: s.payment_status, items: [], ids: [] };
      groups.push(byGroup[key]);
    }
    byGroup[key].items.push(s);
    byGroup[key].ids.push(s.id);
  });
  return groups;
}

function renderSalesList(sales){
  const el = document.getElementById('salesList');
  if(sales.length === 0){
    el.innerHTML = '<p style="font-size:13px;color:#888;">Nenhuma venda registrada ainda.</p>';
    return;
  }
  const groups = groupSales(sales);
  el.innerHTML = groups.map(g => {
    const date = new Date(g.created_at).toLocaleDateString('pt-BR');
    const hasPrices = g.items.every(i => i.unit_price != null);
    const total = hasPrices ? g.items.reduce((sum,i)=> sum + Number(i.unit_price) * i.quantity, 0) : null;
    const itemsHtml = g.items.map(i => `<div>${i.product_name}${i.color ? ' ('+i.color+')' : ''} × ${i.quantity}${i.unit_price!=null ? ' — '+formatMoney(i.unit_price*i.quantity) : ''}</div>`).join('');
    return `
    <div class="sale-row">
      <div class="sale-top">
        <div class="sale-info">
          <div class="sale-name">${g.client_name || 'Cliente não informado'}</div>
          <div class="sale-sub">Conta: ${g.account} • ${date}</div>
          <div class="sale-items">${itemsHtml}</div>
          <div class="sale-total">Total: ${total != null ? formatMoney(total) : '—'}</div>
        </div>
        <button class="icon-btn" onclick="deleteSaleGroup('${g.ids.join(',')}')">Excluir</button>
      </div>
      <div class="sale-controls">
        <select onchange="updateSaleStatus('${g.ids.join(',')}', 'delivery_status', this.value)">
          <option value="Reservado" ${g.delivery_status==='Reservado'?'selected':''}>Reservado</option>
          <option value="Entregue" ${g.delivery_status==='Entregue'?'selected':''}>Entregue</option>
        </select>
        <select onchange="updateSaleStatus('${g.ids.join(',')}', 'payment_status', this.value)">
          <option value="Pendente" ${g.payment_status==='Pendente'?'selected':''}>Pendente</option>
          <option value="Pago" ${g.payment_status==='Pago'?'selected':''}>Pago</option>
        </select>
      </div>
    </div>
  `;
  }).join('');
}

async function updateSaleStatus(idsStr, field, value){
  const ids = idsStr.split(',');
  const { error } = await sb.from('sales').update({ [field]: value }).in('id', ids);
  if(error){ showToast('Erro ao atualizar status', error.message); console.error(error); return; }
  showToast('Status atualizado');
}

async function deleteSaleGroup(idsStr){
  if(!confirm('Excluir essa venda? O estoque já retirado não será devolvido automaticamente.')) return;
  const ids = idsStr.split(',');
  const { error } = await sb.from('sales').delete().in('id', ids);
  if(error){ showToast('Erro ao excluir', error.message); return; }
  showToast('Venda excluída');
  loadSales();
}

/* ---------- PASSWORD ---------- */
async function changePassword(){
  const current = document.getElementById('currentPass').value;
  const next = document.getElementById('newPass').value.trim();
  const errorEl = document.getElementById('passError');
  errorEl.style.display = 'none';

  if(!next || next.length < 4){
    showToast('A nova senha precisa ter pelo menos 4 caracteres');
    return;
  }

  const { data, error } = await sb.from('admin_config').select('password').eq('id', 1).single();
  if(error || !data || current !== data.password){
    errorEl.style.display = 'block';
    return;
  }

  const { error: updateError } = await sb.from('admin_config').update({ password: next }).eq('id', 1);
  if(updateError){
    showToast('Erro ao atualizar senha');
    return;
  }

  document.getElementById('currentPass').value = '';
  document.getElementById('newPass').value = '';
  showToast('Senha atualizada com sucesso');
}

toggleSubcategoryField();
</script>
</body>
</html>

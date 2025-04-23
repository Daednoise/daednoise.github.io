<!DOCTYPE html>
<html>
<head><meta charset="utf-8"><title>Adding to Cart…</title></head>
<body>
<script>
(async()=>{
  const p=new URLSearchParams(window.location.search),
        productId=Number(p.get('pid')),
        sku=p.get('sku'),
        me=await fetch('/api/storefront/customers/me',{credentials:'include'}).then(r=>r.json()),
        inv=await fetch('https://abc.irishtitan.cloud/api/vault/inventory-check?sku:in='+sku).then(r=>r.json());
  if(!inv[0]?.has_inventory) return alert('Out of stock');
  const cart=await fetch('/api/storefront/carts',{method:'POST',credentials:'include',headers:{'Content-Type':'application/json'},body:JSON.stringify({lineItems:[{productId,quantity:1}]})}).then(r=>r.json());
  await fetch('https://abc.irishtitan.cloud/api/vault/cart-reserve',{method:'POST',headers:{'Content-Type':'application/json','X-Requested-With':'XMLHttpRequest'},body:JSON.stringify({cart_id:cart.id,customer_id:me.data.id,customer_email:me.data.email,product_id:String(productId),sku,quantity:1})});
  window.location.href='/cart.php';
})();
</script>
</body>
</html>

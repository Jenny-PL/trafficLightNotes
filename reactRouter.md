```
<Route path="/" element={<App />}>
  <Route path="sales" element={<Sales />}>
    <Route path="invoices" element={<Invoices />}>
      <Route path=":invoice" element={<Invoice />} />
    </Route>
  </Route>
</Route>
```

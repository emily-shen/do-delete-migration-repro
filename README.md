To reproduce:

1. run `npx wrangler deploy`
2. Add a migration with deleted_classes (uncomment in wrangler.jsonc), delete binding, delete DO class.
3. run `npx wrangler deploy`
4. Observe API error: Cannot apply --delete-class migration to class 'MyDurableObject' without also removing the binding
   that references it. [code: 10061]

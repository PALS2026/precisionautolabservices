PRECISION AUTO LAB — VEHICLE INVENTORY EDITOR

This package includes the website, editable vehicle data, existing BMW photos, and a simple private-use inventory manager.

IMPORTANT: This editor uses a GitHub fine-grained personal access token entered by you in the admin page. It does NOT require a paid service or a separate OAuth server. The token is saved only in this browser's local storage after you connect. Use a token limited to this one repository with Contents read/write permission. Do not share it. Disconnect removes it from this browser.

SETUP
1. Upload the contents of this folder to the root of the GitHub repository PALS2026/precisionautolabservices, replacing the existing index.html and adding the admin, content, and uploads folders.
2. Confirm the repository's default branch is main. If it is not, change BRANCH near the top of admin/index.html to the actual branch name before publishing.
3. Netlify should automatically deploy the GitHub commit. Confirm the live website still works.
4. Visit https://precisionautolabservices.netlify.app/admin/.
5. Create a GitHub fine-grained personal access token: GitHub → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token. Resource owner PALS2026; select only precisionautolabservices; Repository permissions → Contents → Read and write. Metadata is read-only by default. Set an expiry, generate, and copy the token.
6. Paste the token into the admin page and click Connect & load inventory.

The public site reads content/vehicles.json. New photos are uploaded into uploads/. Saving inventory creates a GitHub commit, which triggers Netlify's automatic deploy. The editor can add, edit, delete, hide, and mark vehicles sold.

If the Netlify deploy branch is not main, change BRANCH in admin/index.html to match it. Keep your token private. Anyone with this token can edit the repository contents allowed by its scope.

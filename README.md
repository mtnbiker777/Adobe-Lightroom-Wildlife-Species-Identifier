# Adobe-Lightroom-Wildlife-Species-Identifier
This is an Adobe Lightroom classic plugin for bird, and nature photographers. It takes your photo directly from inside Lightroom Classic and sends it to Google's advanced Gemini Vision AI to identify species and allows you to write precise keywords directly to your images.

What previously took minutes of exporting, uploading to tools like iNaturalist, and manually copying tags can now be done in seconds without ever leaving Lightroom. Because keywords are applied directly to the image, typos are eliminated completely. Here's a sample of what you get back!

<img width="756" height="627" alt="image" src="https://github.com/user-attachments/assets/3741b302-72c4-4b20-ac62-12f3bd2cbffc" />

Download the plugin today and test it on 10 wildlife photos for free. If you find it saves you time you can unlock an unlimited lifetime license for $30 CAD.

The model analyzes plumage, markings, body geometry, date, and GPS location metadata to identify a broad range of biological classes:

<ul>
<li>Birds (Avian): Identifies species, visible plumage variations (breeding/non-breeding), life stages, and sexual dimorphism.
<li>Mammals : Carnivores, ungulates, rodents, marine mammals, and small field mammals.
<li>Insects & Arthropods : Butterflies, moths, odonata (dragonflies/damselflies), beetles, bees, wasps, and arachnids.
<li>Reptiles & Amphibians : Snakes, turtles, lizards, salamanders, toads, and frogs.
<li>Plants & Trees : Wildflowers, trees, shrubs, grasses, ferns, leaves, bark, and seasonal fruit/berries.
<li>Fungi & Marine Life : Mushrooms, bracket fungi, lichens, freshwater fish, mollusks, and crustaceans.
</ul>

Google Gemini API & Performance Limits
The plugin connects directly to Google AI Studio using your own personal API key. For most photographers, the Free Tier offers plenty of capacity:

<ul>
<li>15 Requests Per Minute (RPM): Process up to 15 images within any rolling 60-second window.
<li>1,500 Requests Per Day (RPD): Generous daily limit that resets every midnight Pacific Time.
<li>Optimized Image Payload: Images are automatically resized locally between 300 KB and 5 MB (configurable in your plugin preferences) before uploading to ensure fast transfer speeds.
<li>Location & Date Accuracy: EXIF capture date, time, and GPS coordinates are submitted with the image payload, allowing the AI to factor in regional migration and seasonal range maps for higher identification accuracy.
<li>Data Handling: On Google's Free Tier, prompts and images may be reviewed by automated systems to train models. If strict data confidentiality is required, connecting a paid Google Cloud billing account disables model training logs.
</ul>
<p>Learn more about Google's setup: <a href="https://ai.google.dev/gemini-api/docs/api-key" target="_blank" rel="noopener">Google API Key Setup Guide</a> | <a href="https://aistudio.google.com/docs/pricing" target="_blank" rel="noopener">Google AI Studio Pricing</a>.</p>

For detailed installation instructions see <a href="https://jgalea.com/wildlife-identifier/">My detailed help page.

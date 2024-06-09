## Hi there 👋

Currently working on :: <span id="workingOn"></span>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    // Replace 'your-json-url' with the actual URL of your JSON
    const url = 'https://your-server.com/your-json-url';

    fetch(url)
        .then(response => {
            if (!response.ok) {
                throw new Error('Network response was not ok ' + response.statusText);
            }
            return response.json();
        })
        .then(data => {
            // Assuming 'workingOn' is a key in your JSON
            const workingOnContent = data.workingOn;
            if (workingOnContent) {
                document.getElementById('workingOn').textContent = workingOnContent;
            } else {
                console.error('workingOn key not found in the JSON');
            }
        })
        .catch(error => {
            console.error('There has been a problem with your fetch operation:', error);
        });
});

</script>
<!--
**Echo-noen/echo-noen** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

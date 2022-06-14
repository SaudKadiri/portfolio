<script>
    import global from '../global.css'
    import Fields from "../components/Fields.svelte";

    let fields = [
        {
            title: 'About Me',
            description: 'Hey, I\'m Saud. I\'m a Computer Engineer and I do System programming. I\'m also highly skilled in the field of AI. \
            I have practiced Data Structures and Algorithms throughly. I\'m interested in Computer Architectures(ARM), Extended Reality(XR), and some low-level computer things. \
            I prefer using Unix-based Operating Systems; currently using Apple macOS(Darwin) and have experienced Ubuntu(Debian), WSL and Fedora in the past. \
            Other than computer science I love Philosophy, Nature and my introvert personality. I also like to maintain a personal diary.',
        }, 
        {
            title: 'Skills',
            description: 'These skills were gained by me throughout my educational days. \
            This is NOT to scale and has been included with the intention of displaying my relative strength / knowledge in each. \
            Also to rectify, these are not the only skills that I know; but are only to show some of my favorites.'
        }, 
        {
            title: 'Projects',
            description: 'I love doing projects and I always give 100% to my team. I like to put my team first and than myself. \
            I\'ve been experienced of both Project leader and lead software developer throughout the projects.'
        }, 
        {
            title: 'Education',
            description: 'I believe that Computer Education is gained more by the SEEKER (self-lerner, i.e. Online) than the COLLEGE-ATTENDER. \
            I gained most of my knowlege gained by reading books/documentation, watching Coursera/edX/YouTube/Conferences, and then College. \
            Above I\'ve listed some of the books/courses that helped me a lot.'
        },
        {
            title: 'Contact Me',
            description: 'The above are the ways to contact me.'
        },
        {
            title: 'This Webiste',
            description: 'Even if I\'m not a professional Web Developer, I\'m a true Computer Engineer. So I decided to make this website for my love i.e. Computer Science\
            I know there are lakhs of better portfolios than mine; still I\'m truly glad to have made it by my own... I could have had a simple HTML page itself... but I care for UI. \
            I initially decided to make the Portfolio using Plain HTML, CSS, JS but it bored me. Then I decided to use Django, but it just never went forward, then came React; \
            which I felt was unnecessarily complex, so I ended up using SvelteKit. This project is made using SvelteKit and hosted on Google Cloud (for free). \
            The source code for this website is open-source and is available on my github(like most of my projects).'
        }
    ]
</script>



<main class="container">
    <Fields {fields}/>
</main>
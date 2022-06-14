<script>
    import global from '../global.css'
    import Fields from "../components/Fields.svelte";

    // let fields = ['Programming Languages', 'Frameworks and Tools', 'App development', 'Courses']
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
            description: ''
        }
    ]
</script>



<main class="container">
    <Fields {fields}/>
</main>
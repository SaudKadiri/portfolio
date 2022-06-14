<script>
    import global from '../global.css'
    import Fields from "../components/Fields.svelte";

    // let fields = ['Programming Languages', 'Frameworks and Tools', 'App development', 'Courses']
    let fields = [
        {
            title: 'About',
            description: 'Hey, I\'m Saud. I\'m a Computer Engineer and I do System programming. I\'m also highly skilled in AI. I have practiced Data Structures and Algorithms throughly. I\'m interested in Computer Architectures(ARM), Extended Reality(XR), and low-level computer things. I prefer using Unix-based Operating Systems; currently using Apple macOS and have experienced Ubuntu(Debian) and Fedora in the past. Other than computer science I love Philosophy, Nature and "Good" people.',
        }, 
        {
            title: 'Skills',
            description: ''
        }, 
        {
            title: 'Projects',
            description: ''
        }, 
        {
            title: 'Education',
            description: ''
        }, 
        {
            title: 'Profiles',
            description: ''
        }
    ]
</script>

<main class="container">
    <Fields {fields}/>
</main>
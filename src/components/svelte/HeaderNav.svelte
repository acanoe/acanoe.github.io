<script>
    export let currentPage;
</script>

<nav>
    <ul>
        <li class:active={currentPage == "home"}>
            <a href="/">
                <span>Home</span>
                <svg aria-hidden="true" focusable="false">
                    <use xlink:href="#icon-chevron-right" />
                </svg>
            </a>
        </li>
        <li class:active={currentPage == "resume"}>
            <a href="/resume">
                <span>Resume</span>
                <svg aria-hidden="true" focusable="false">
                    <use xlink:href="#icon-chevron-right" />
                </svg>
            </a>
        </li>
        <li class:active={currentPage == "blog"}>
            <a href="/blog">
                <span>Blog</span>
                <svg aria-hidden="true" focusable="false">
                    <use xlink:href="#icon-chevron-right" />
                </svg>
            </a>
        </li>
        <li class:active={currentPage == "experiments"}>
            <a href="/experiments">
                <span>Experiments</span>
                <svg aria-hidden="true" focusable="false">
                    <use xlink:href="#icon-chevron-right" />
                </svg>
            </a>
        </li>
    </ul>
</nav>

<style>
    nav ul {
        list-style: none;
        display: flex;
        flex-direction: column;

    }

    li {
        padding: 0 .5rem;
        border-radius: 1rem;
    }

    .active {
        background: hsla(var(--accent-h), var(--accent-s), 90%);
    }

    a {
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin: 1rem 0;
        text-decoration: none;
        color: var(--accent-color);
    }

    a svg {
        height: 1.1rem;
        width: 1.1rem;
    }
</style>

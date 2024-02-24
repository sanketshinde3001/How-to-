# How to add scroll button

1) Install react-scroll package
    ```js
    npm install react-scroll
    ```
2) Basic Structure where we want to add button
    ```js
    import { Link } from 'react-scroll';

    const ScrollButton = () => {
        return (
        <Link
            to="footerSection"  // Replace with the ID of your footer section
            smooth={true}
            duration={500}
        >
        <button className="px-6 py-3 bg-purple-700 text-white rounded-3xl font-semibold
        cursor-pointer  xl:mb-60">
                Let's Partner Together
        </button>
        </Link>
        );
    };
    export default ScrollButton;
    ```
    
3)    Add id to div to footer
        ```js
        <div id="footerSection">
        // footer code
        </div>
        ```
    
    
